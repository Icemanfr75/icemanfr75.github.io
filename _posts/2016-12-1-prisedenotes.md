---
layout: post
title: Tuto/Critique - Les outils de prise de notes
category: geek, tuto
tags: android, développement, geek, Geekeries, iOS, logiciel libre, notes, programmation, Tutoriel
---
**La prise de note, surtout sur mobile, est devenu le nouveau terrain de jeu des <span style="text-decoration:underline;"><a href="https://fr.wikipedia.org/wiki/Gafa">GAFAM</a>. Google a sorti son Keep, après Microsoft et son OneNote, lesquels concurencent Evernote dont le portage est presque global....sauf sur GNULinux. **

L'engouement est tel pour ce type de produit que Framasoft a réagi récemment avec <span style="text-decoration:underline;"><a href="https://framanotes.org/">Framanotes</a>, dont je parlerai plus loin. L'intérêt est d'avoir accès à des documents courts, voir éphémères, des notes, voir des mots de passe (attention danger!), etc... et de pouvoir les partager sur tous ses terminaux, du PC, à la tablette en passant par le smartphone, de Dunkerque à Tamanrasset en passant par Papeete. Qui dit partage dit donc mot de passe pour accéder à son compte, mais aussi des clauses sur l'accès aux données personnelles de la part de l'hébergeur. Cela signifie vulnérabilité des données, ce qui a été avéré en 2013 pour Evernote.

Il y a différents niveaux de prise de note, entre celui qui ne fonctionne qu'en mode texte (je m'en contente bien, personnellement), ou celui qui permet aussi les notes sonores, l'intégration de photos, l'annotation sur des images, etc....Evernote a pris le leadership avec ces vastes possibilités mais on voit un produit concurrent émergé dans le logiciel libre : <span style="text-decoration:underline;"><a href="https://turtlapp.com/">**Turtl**</a> ! C'est ce choix qu'a fait Framasoft avec son service Framanotes, tout prêt pour qui le veut. Il suffit alors de suivre l'aide pour accéder à ses notes via Android. Enfin ça, c'est la théorie. J'avais testé turtl a à ses débuts et c'était bien trop lent. Aujourd'hui, ce n'est plus le cas et l'application est rapide à se lancer, fluide et suffisamment complète par rapport à Evernote. Evernote est d'ailleurs devenu excessivement lourd et ne bénéficie pas des même fonctions sur mobile et en version web, ce qui est inadmissible aujourd'hui. Je ne parle même pas de l'usine à gaz OneNote, qu'on essaye vainement de m'imposer au travail. Le problème de Turtl, aujourd'hui, vient de bugs de connexion sur mon mobile en KitKat, qui oblige à remettre son mot de passe toutes les 30 s.... A tester donc avec le votre. Sinon, vous avez, avec le tutoriel de Framasoft, la possibilité de l'installer sur votre propre serveur, mais là, attention : Il vous faudra maîtriser la sécurité de votre serveur ou bien réfléchir à ce que vous y mettez.

Et puis il y a des outils de prise de note très simples, en format texte ASCII, avec même des possibilités de chiffrer ses notes pour qu'elles ne tombent pas en de mauvaises main. J'ai fait le choix de la simplicité ultime avec **<a href="https://github.com/openintents/notepad">OI Notepad</a>**, un fork d'un vieux produit intégré dans Android à ses débuts, dont les code source est disponible. L'avantage est que l'on peut créer une note et la sauvegarder n'importe où dans l'arborescence de fichiers de son smartphone. Le format est lisible par n'importe quoi, mais revers de la médaille, il n'est pas possible de chiffrer tout cela aujourd'hui, ou de synchroniser cela avec son PC(sinon à travers un autre outil installé). Je n'y garde donc que des petites choses peu personnelles, pas importantes si ce n'est que je dois les avoir sur moi. Une liste de course, par exemple, peut être gardée comme cela. Autre possibilité un peu plus perfectionnée : <a href="https://apps.owncloud.com/content/show.php/ownNote+-+Notes+Application?content=168512"><span style="text-decoration:underline;">**OwnNote**</a>, le client de note sous Android pour les serveurs dotés de <span style="text-decoration:underline;"><a href="https://cheziceman.wordpress.com/2016/01/23/tutotest-owncloud-ou-le-long-chemin-restant/">Owncloud</a>. Là encore, on est sur du produit libre, simple d'usage, mais qui évidemment nécessite un serveur dûment protégé. J'avais testé cela avec la mère Zaclys et ça fonctionne toujours très bien. On peut éventuellement reprocher le manque de fonction de tri automatique par divers critères, le coté austère, l'absence de gestion des tags. Ca ne me manque pas....Mais ici, on est synchronisable entre tous ses terminaux.

Après, j'ai aussi testé deux autres produits privateurs : **Gnotes** et **ColorNote** sous Android. Ils fonctionnent tous les deux très bien avec la synchronisation de différents terminaux. Pour le second, seuls les téléphones/tablettes sont pris en compte alors que le premier dispose d'une application web. Mais par contre, Colornote se distingue par quelque chose d'essentiel pour moi : L'export sur carte SD et la possibilité aussi de ne garder que le mode offline. Colornote dispose aussi d'une protection des données par mot de passe local. Mais les conditions d'utilisation précisent bien que nos données peuvent être lues et exploitées par l'hébergeur.

Si je devais faire une **cahier des charges de l'application idéale**, il y en aurait 2, selon l'utilisation. Pour la plus complète, ça serait :

* Saisie texte avec style (bras, italique, souligné, barré + taille, au minimum)
* Mode saisie de liste à cocher
* Champ titre séparé du reste
* Application web, Android, iOS...
* Sauvegarde périodique et automatique sur SD externe (et pas SD interne) et/ou sur serveur personnel
* Possibilité de chiffrement avec GPG
* Export possible des notes en format ascii
* Utilisation de l'arborescence fichier de l'OS sur terminal mobile
* Partage des notes via mail ou autre
* Gestion des étiquettes
* Gestion des couleurs
* Synchronisation entre terminaux via serveur autohébergé
* Insertion d'images avec découpe
* Insertion de commentaires libres, vectoriels ou texte
* Mode "enregistreur audio"

Pour la plus simple :

* Saisie en mode texte sans style
* Champ titre séparé du reste
* Sauvegarde périodique et automatique sur SD externe (et pas SD interne)
* Possibilité de chiffrement avec GPG ou à minima avec mot de passe
* Export possible des notes en format ascii
* Partage des notes via mail ou autre

&nbsp;

Bref, dans tous ces cas, les applications du marché ne remplissent pas le cahier des charges, soit par manque de liberté ou fermeture, soit par manque de fonction. Alors qui s'y colle?
