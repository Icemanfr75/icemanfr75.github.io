---
layout: post
title: Photo - La tête dans les nuages
category: tuto, geek
tags: backup, blog, cloud, Geekeries, hébergement, owncloud, photographie, Tutoriel
---
**L'été est une période riche en photos et il faut penser à les sauvegarder, voir à les partager (pour bien pourrir la vie de ses amis). Mais entre le rachat de Yahoo par Verizon, donc de Flickr, et le remplacement de Picasaweb par l'infâme Google Photos, c'est l'occasion de se poser les bonnes questions.**

J'utilise encore Flickr et sa formule 1To gratuit avec le respect du creative commons qui n'a pas de comparaison. Malheureusement, je ne donne pas cher de la peau de ce service dans les mains de l'opérateur téléphonique Verizon. Déjà, l'outil PC de synchronisation est devenu payant, et les bugs de transferts persistent depuis plus de 10 ans. Ce n'est peut être pas un GAFAM mais ça pourrait s'en rapprocher. Pas question pour moi d'utiliser un Google Drive/photos , un produit Microsoft équivalent, etc... J'ai un NAS qui héberge mes photos avec sauvegarde redondante et aucune ouverture sur l'extérieure. Ça plus une sauvegarde ponctuelle sur un disque externe en plus et ça parait déjà pas si mal. Mais si parfois je veux accéder à du contenu hors de chez moi, j'ai aussi la solution MEGA dont l'outil de synchronisation fonctionne vraiment bien en Windows, Android, ....et je ne l'ai pas mis sur ma Debian mais <span style="text-decoration:underline;"><a href="https://mega.co.nz/linux/MEGAsync/">il existe</a></span>. 50Go, c'est déjà pas mal, surtout si on se contente d'une résolution pas trop gourmande pour ce backup.

**Utilisation au quotidien**

Quand on n'est pas un pro, la sauvegarde des photos et la diffusion éventuelle peuvent attendre d'être tranquillement à la maison. Donc inutile de penser à mettre ses photos non triées synchronisées automatiquement de son smartphone/PC sur un service de cloud. ça, Cozy ne l'a pas encore bien compris dans sa <span style="text-decoration:underline;"><a href="https://cheziceman.wordpress.com/2016/07/12/test-owncloud-vs-cozycloud-les-liberateurs-du-nuage/">version mobile actuelle</a></span>, pour ceux qui voudraient s'auto-héberger, mais ça va venir. Il faut dire que copier les Apple/Google dans le domaine n'est pas toujours une bonne idée. A force d'infantiliser l'utilisateur, on en vient à des aberrations et surtout des abus sur la propriété des photos. Synchroniser ne signifie pas balancer tout dans un répertoire et trier ensuite dans une interface Web

**L'heure du Choix**

Donc une fois chez soi, on peut trier, sauvegarder d'abord en local (avec la fameuse <span style="text-decoration:underline;"><a href="http://genma.free.fr/?Sauvegarde-la-regle-des-3-2-1">règle des 3-2-1</a></span>) puis hors de chez soi (chez un ami, ou bien chez un hébergeur sûr). Reste donc à trouver un hors de chez soi de confiance. A moins qu'un généreux ami vous fasse cadeau de gigaoctets de données sur son serveur, il va falloir trouver quelqu'un de sûr. J'ai cité Mega mais on ne peut pas dire que ça soit très sûr quand même quand on connaît l'histoire de la société et ce qu'il y a derrière aujourd'hui (un richissime chinois en difficulté avec le pouvoir). Reste donc la solution d'un bon hébergeur fiable, notamment économiquement, et qui offre la possibilité de s'installer son petit Ownloud à soi sans trop de galère. Je n'ai pas choisi pour l'instant mais je ne pense pas que j'irai chez la mère Zaclys, malgré tout le sérieux de l'association (limitation à 9 ou 12Mpix et 250 à 500Mo par transfert). Avec 45go à transférer (voir moins si je réduis la résolution), je n'ai pas envie de galérer trop longtemps. Reste aussi à tester la robustesse de l<span style="text-decoration:underline;"><a href="https://owncloud.com/products/desktop-clients/">'outil desktop</a></span> en windows et debian.

**Owncloud Desktop ?**

De ce coté là, pas de souci à partir de fichiers sur son PC. Enfin si....Car la seule option locale est d'utiliser un répertoire dans lequel on a les photos en sous répertoires, mais impossible d'avoir des sources hétérogènes ou une structure différente d'un répertoire ne s'appelant pas Photo pour les photos. Comme j'utilise le NAS comme support primaire, et les PC de la maison comme clients uniquement, c'est problématique car je ne veux pas polluer ma structure de fichiers. En plus, je ne peux pas choisir de mettre en pause la synchro sur des branches de l'arborescence et laisser les autres en veille active. On ne peut modifier ou éditer sa synchronisation pour changer le répertoire. Il faut supprimer et recréer. De ce coté là, Mega est bien plus évolué avec des choix de synchronisation dignes d'un logiciel dédié comme syncbackSE sous windows, par exemple (pas libre pour un sou, par contre). Disons le clairement, Owncloud est à peu près aussi mal foutu que 90% des outils du marché, notamment ceux de Box.net, Dropbox, ou de Microsoft. Le jour où les développeurs comprendront que l'utilisateur doit être celui à prendre en compte avant leur propre désir, on aura fait un grand pas. Et à force de copier l'idiotie du leader, on en arrive à ce nivellement par le bas.

**Conclusion**

C'est assez désespérant mais si je veux utiliser une solution libre et hébergée, je ne vais pas pouvoir utiliser l'outil officiel de synchronisation. Pour un utilisateur lambda, la synchronisation est déjà complexe à expliquer avec les différentes règles d'exclusions. Mais si en plus on n'a pas tous les outils pour faire ça, il ne reste que : Refaire toute sa structure de sauvegarde et se plier aux exigences d'un développeur autiste, vendre son âme à une société, se faire des amis acceptant d'héberger vos données. En l'état, je reste donc encore sur la solution actuelle. Mais je suis sûr que quelqu'un aura une autre idée en pensant à la fameuse madame miche.