---
layout: post
title: Tuto - Degooglisation de contacts sur Mobile
category: tuto
tags: android, contact, degooglisation, geek,
---
**Il y a quelques temps, je pestais contre le manque de finition de la <a href="https://cheziceman.wordpress.com/2016/01/23/tutotest-owncloud-ou-le-long-chemin-restant/">solution Owncloud</a>, pour héberger ces données. Mais la plupart des problèmes venait aussi de l'adéquation entre la logique d'Android et celle d'Owncloud. Il faut donc revenir au source, l'initialisation de son smartphone.**

Car tout est fait pour aller chez Google lorsqu'on démarre son smartphone pour la première fois. On a donc inséré sa **carte sim**, sur laquelle il y a peut-être des contacts issus de son ancien téléphone, avec des noms raccourcis et des données manquantes. Voilà donc le premier lieu où se trouvent vos contacts. Le téléphone propose en général de les rapatrier sur sa propre **mémoire interne**, car il en a des Gigas à revendre. Et vous voilà avec un clone de vos données sur le téléphone. Et puis viens l'étape où l'on saisit son compte Google pour synchroniser ses données, ou bien le créer si l'on en a pas....Et voilà les données qui partent encore à un autre endroit, dans **Gmail**.

Si on veut éviter cela, il va falloir ruser. On va imaginer que vous avez votre hébergement quelque part avec une instance owncloud ou baikal, ....ou autre, si ça se trouve, mais compatible <a href="https://fr.wikipedia.org/wiki/WebDAV">WebDAV</a>. Ah, j'en ai déjà perdu ? Qu'importe le nom finalement, c'est un protocole qui a donné naissance à des dérivés baptisés CardDAV pour les contacts et CalDAV pour les calendriers et agendas. Vous avez donc un serveur quelque part capable d'heberger tout cela, et c'est tant mieux. Mais votre Smartphone android n'a pas les outils pour s'en sortir tout seul et il va falloir l'aider. Surtout que le seul moyen de rajouter une application est le ...Google Play, donc avec un compte Google. Quand je vous disais qu'ils sont vicieux ! Premier réflexe, aller chez F-Droid et télécharger l'APK.

* Sauf que pour l'installer, il faut aller dans les &lt;Réglages&gt;, Rubrique &lt;Sécurité&gt; puis descendez jusqu'à &lt;Administration du périphérique&gt; pour cocher &lt;Sources inconnues&gt; et décocher &lt;Vérifier les applications&gt;. Ne vous inquiétez pas, vous pourrez tout enlever après.
* Donc ensuite, allez chez <a href="https://f-droid.org/">F-Droid</a>, un market alternatif qui propose de télécharger son application. Et là, vous avez un joli fichier apk qu'il faut lancer et accepter l'installation.
* Après avoir téléchargé la base de données, vous pouvez chercher <a href="https://f-droid.org/repository/browse/?fdfilter=davdroid&amp;fdid=at.bitfire.davdroid">DavDroid</a> et l'installer de la même manière.
* Vous le lancez et après le message d'appel aux dons, vous cliquez sur la petite clé avec un "+" en haut à droite pour créer un compte utilisateur. Trois questions à répondre : L'adresse du serveur (là je ne peux rien pour vous, si ce n'est vous dire de prendre du https), le nom de l'utilisateur et le mot de passe. En dessous il y a une case à cocher ou pas. Tentez les deux, selon votre type de serveur, ça ne fait pas mal.
* Voilà, vous être prêt !

![davdroid](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2016/davdroid.jpg)

Mais prêt pour quoi ? Pour vous faire chier entre les trois (voir quatre si vous avez aussi un compte google) sources de contacts installés sur ce smartphone qui vous hait profondément. Ouvrez l'application Contacts et allez dans les Filtres (les trois petits points puis Filtrer )... Là, ça dépend de beaucoup des marques, mais il se peut qu'il y ait un cumul entre les contacts de la carte Sim, ceux du téléphone (contact local), ceux de Google, ceux de DAVdroid, etc.... Là, il va falloir choisir son camp, c'est à dire celui de DAVdroid. C'est maintenant là que tout se passera pour vous et le téléphone ne le sait pas encore.

* Allez dans ce menu et faire "Importer des contacts"
* Sélectionnez la source entre "Carte SIM" ou "Mémoire Interne"
* Sélectionnez ensuite la destination en prenant "DAVDroid"

Et si vous avez des contacts google alors ? Et bien c'est la merde.... Non, il suffit d'abord de les exporter vers la mémoire interne dans un format VCF... Puis de faire ce qu'il y a au dessus ensuite.

![contact](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2016/contacts.jpg)

Voilà on y est presque. Il n'y a plus qu'à synchroniser tout ça avec le serveur en allant dans les réglages, rubrique synchronisation et de faire la synchro avec le serveur. Vos ennuis ne sont pas terminés car lorsque vous allez créer un nouveau contact, il faudra faire attention à :

* Sélectionner le bon emplacement, c'est à dire DAVDroid
* Entrer les bons champs qui ont la désagréable habitude de ne pas être les mêmes que lorsque c'est un compte Google, Téléphone ou SIM.... Remplissez les champs "Nom" et "Prenom", ce dernier n'étant visible qu'avec la petite flèche vers le bas sous des termes comme "Prénom en phonétique".

Il ne vous reste plus qu'à retourner dans la rubrique filtrer et faire disparaître le superflu. Je vous conseille également d'aller sur votre PC préféré pour éditer les contacts de manière confortable. Mais comme justement vous avez aussi les mêmes dessus, ça sera l'occasion de tout unifier. Alors, vous voyez que c'est pas dur de se dégoogliser !
