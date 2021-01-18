---
layout: post
title: Blog et tuto - Pourquoi Rechercher simple quand on peut Rechercher compliqué ?
category: tuto, geek
tags: catfish, debian, Geekeries, gnome search tool, linux, logiciel libre, recherche, Tutoriel
---
**Le monde du logiciel libre m'étonnera toujours et certains archaismes en sont la preuve.**

J'ai dans la tête de convaincre une windowsienne invétérée de passer à Ubuntu/Mint voir Debian dans une prochaine machine. Mais pour cela, il faudrait qu'à minima, elle puisse survivre sans moi dans ce monde hostile et ...libre. Et là, je suis tombé sur un truc que je n'avais pas fait depuis longtemps et qui m'a posé problème sur ma Debian XFCE préférée :

 * J'ai des fichiers que je veux supprimer sur au moins 20 répertoires d'un disque dur réseau préalablement monté (en auto au démarrage). Ces fichiers ont tous la même racines qu'on appelera toto...
 * Sous windows ou autre système je n'aurais qu'à faire un toto*.* dans le champ de recherche de l'explorateur/fenêtre du disque pour que ça m'affiche tous les fichiers potentiellement concernés.
 * Ensuite je n'aurais qu'à sélectionner les fichiers concernés et faire un supprimer.

Sauf que là, Thunar, le gestionnaire de fichier de XFCE n'a pas de fonction de recherche. Catfish,un outil de recherche, ne permet pas ensuite de supprimer les fichiers trouvés mais on peut l'intégrer à Thunar en menu contextuel. Encore faut-il installer catfish d'abord qui n'a pas été prévu dans le package de base! Je n'aurais pas ce problème dans un environnement Gnome, évidemment...

A ce moment, je me pose vraiment la question de savoir si on marche sur la tête. J'ai trouvé par ailleurs une autre solution en passant par un vrai gestionnaire de fichier, comme double commander, un clone de <a href="http://frederic.bezies.free.fr/blog/?p=14858">T</a><a href="http://frederic.bezies.free.fr/blog/?p=14858">otal Commander,</a></span> soit donc un clone de norton commander, outil datant de ... 1986, soit 30 ans! En 30 ans, il n'est pas venu à l'idée des mecs derrière XFCE et Thunar qu'on pourrait simplement chercher des fichiers et vouloir les supprimer, un truc basique qu'on peut aussi faire par ligne de commande, comme il y a 40 ans. Mais franchement, dans quel monde vivent ces gens?

Bilan, je peux aussi utiliser le gnome-search-tool, ou bien encore mettre carrément gnome, ce qui revient à mettre à genou une vieille machine pour juste avoir une fonction de base d'un OS. Même mon vieux BeOS en R5 avait cette fonction, et je ne parle même pas de Directory Opus sur Amiga ! Ah mais par contre, pour grogner sur systemd et autres conneries dont 99% des usagers normaux se foutent, il y a du monde, et pour faire des forks inutiles aussi. Je ne suis pas le seul à le penser si j'en crois le forum XFCE ou un magazine sur le logiciel libre :

![image](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2016/xfceforum1.jpg)

![image](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2016/xfce2.jpg)

Je ne compte pas le nombre de sujets sur les forums anglais sur cette fonctionnalité avec l'ajout de plugin à Thunar mais qui ne vont pas au bout du sujet, à savoir dire si on peut ou pas manipuler les fichiers du résultat. Des demandes d'évolutions trainent depuis au moins 4 ans, chacun se renvoyant la balle entre catfish, thunar, gtk, ...

Donc je m'en vais expliquer maintenant comment rajouter une fonctionnalité  à sa Debian XFCE qui devrait être en standard et ne l'est pas parce que ça appartient à la chapelle d'à coté (Gnome en l'occurence)

![image](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2016/thunarsearch.jpg)

Donc au préalable, dans synaptic, vous pouvez installer **gnome-search-tool** (ou bien la ligne de commande mais bon c'est pas le but). Ensuite, dans le gestionnaire de fichier (donc Thunar), il faut faire &lt;Editer&gt; et &lt;Configurer les actions personnalisées...&gt;, puis appuyer sur le bouton &lt;+&gt; avant de renseigner comme ce qui suit :

<pre class="bbcode_code">Nom: Rechercher des fichiers

Description: Commencer la recherche ici

Commande: gnome-search-tool --path %f

icone: /usr/share/icons/Tango/scalable/actions/search.svg

</pre>

Ne reste plus qu'à aller dans l'autre onglet de la boite de dialogue et cocher Dossier en laissant le champs à *. Ainsi une fenêtre de recherche s'ouvre et donne un résultat possible à exploiter en suppression et ....c'est tout. Un peu léger.

La seule autre solution est de passer par Double Commander, installable avec les commandes suivantes (pour une debian 7.0, <a href="http://software.opensuse.org/download.html?project=home%3AAlexx2000&amp;package=doublecmd-gtk">source avec autres cas</a></span> )

<pre>echo 'deb http://download.opensuse.org/repositories/home:/Alexx2000/Debian_7.0/ /' &gt;&gt; /etc/apt/sources.list.d/doublecmd-gtk.list

apt-get update

apt-get install doublecmd-gtk</pre>

Et ça donnera ça au final :

![image](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2016/doublecommander.jpg)

A noter qu'une fois le résultat afficher, il faut "l'exporter" vers un onglet, pour pouvoir effectuer toutes les manipulations souhaitées. C'est un peu rébarbatif pour les adeptes de la modernité et du drag and drop, mais ça marche.

Maintenant, y aura-t-il enfin une personne sensée dans ce monde pour intégrer ça en dur dans Thunar sans passer par un outil gnome qui lui même utilise les commandes unix ou par un autre produit finalement plus lourd ? Parfois j'en doute.


