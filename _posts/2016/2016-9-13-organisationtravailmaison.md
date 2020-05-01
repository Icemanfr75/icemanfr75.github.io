---
layout: post
title: Blog - Repenser son organisation de travail... à la maison
category: geek, tuto
tags: backup, blog, box, geek, Geekeries, mega, sauvegarde, tutoriel, Tutoriels
---
**Au départ, je pensais consacrer mon année à revoir petit à petit l'emplacement de mes données. Mais peu à peu, je revois aussi ma manière de travailler, faisant converger habitude professionnelle et personnelle. Mais non, je ne vais pas parler de télétravail... (encore que des accords sont de plus en plus fréquents dans ce sens dans les entreprises)**

Mon **activité professionnelle** m'amène à me déplacer dans plusieurs bâtiments, autant dans des bureaux que dans des installations industrielles, des environnement sales, pas très compatible avec l'informatique, surtout que j'ai d'autres matériels (fragiles) à transporter. Contrairement à beaucoup de mes collègues, je privilégie ma mobilité et je laisse bien souvent le PC portable entre deux des zones bureaux. Donc il me faut avoir accès à mes documents en ligne sur les autres postes de l'entreprise. Car ma boite a un système de partage de documents qui a des défauts (t'as intérêt à savoir ce que tu cherche), mais aussi la qualité d'être accessible partout (via du VNC aussi ). Du cloud privé en quelque sorte.

**A la maison**, on a historiquement l'habitude d'avoir ses documents sur son ordinateur. Mais j'ai mis en place une réplication (sauvegarde) du répertoire perso sur le NAS qui lui même n'est pas accessible de l'extérieur (pas de besoin, et par sécurité). J'ai aussi fait une réplication de documents sur des services comme Box, Mega, ou un Owncloud de Zaclys, selon la criticité et le type de document, voir en croisant certains. Cela me permet alors de les consulter (rare), pas de les modifier (jamais eu le besoin). J'ai par ailleurs des notes que je classe en deux types : Ephémères sur une appli Android avec sauvegarde sur SD, et Durables sur le Owncloud ( bientôt Nextcloud). Enfin, ponctuellement, je fais des sauvegardes du NAS sur un disque externe, pour les documents critiques. Tout cela amène aussi à une certaine rigueur dans le classement des documents de chaque PC, pour qu'ils soient bien pris en compte.

Mais lorsqu'on regarde l**'évolution des terminaux**, on s'oriente vers des disques plus réactifs  (SSD) mais plus petits pour les terminaux les moins chers, tandis que le haut de gamme garde un certain conservatisme technique. Comme je recherche l'économie dans la consommation d'énergie tout autant que la fiabilité, je regarde un peu plus ce qui se fait dans les terminaux pro, occasion récente comprise. Cela sous entend aussi de ne pas prendre des disques SSD en mode TLC et QLC, soient les moins chers du marché, mais de préférer des disques en SLC ou MLC au maximum. Alors là, c'est rare ! Cela peut paraître de la surqualité au vu des cycles d'écriture-lecture subits, mais j'aime à penser que l'obsolescence programmée en vogue partout va aussi se nicher dans les SSD. La garantie 10 ans ne remplacent pas les données ou le temps passé à réinstaller. Ma paranoïa me pousse à privilégier une sauvegarde des documents sur un serveur (soit en travaillant directement dessus, soit en fin de session de travail par un upload), mais par contre, un peu moins d'utiliser Office365 ou Google Drive, pour ne citer qu'eux. Le choix des prestataires de cloud nécessite un compromis entre la pérennité de la société et sa politique sur les données.

<img class="alignnone size-full wp-image-7461" src="https://cheziceman.files.wordpress.com/2016/09/backup.jpg" alt="backup" width="582" height="615" />

Je m'oriente donc vers un travail client/serveur pour mes documents usuels non critiques. Mais je ne veux pas non plus d'une réplication aveugle façon icloud, boxsync qui prennent tout ce que l'on met dans un terminal et les classent à leur sauce, voire ne les classent pas. Comme dans ma profession, le travail d'archivage de document nécessite **une réflexion en amont sur le classement le plus efficace**. Mais on peut aussi avoir des systèmes avec des tags/etiquettes permettant une double entrée entre thème et répertoire/dossier. Par exemple, si je fais une lettre à ma banque, vais-je la classer dans courrier ou dans banque/finance, ou alors les deux ? La règle de sauvegarde prend aussi du sens quand on pense à la validité du document dans le temps. Professionnellement, les documents sont effacés entre 3 et 10 ans après, voir plus lorsqu'une norme l'impose. Mais chez soi, on ne pense pas à cela, sinon pour la conservation des feuilles de paye, pour les impôts, etc... Là encore, on numérise rarement nos documents, on laisse parfois ses comptes dans le "coffre fort numérique" de sa banque et on n'a pas besoin d'y accéder tous les jours. Ce sont toutes ces réflexions qu'il faut finalement avoir quand on classe ses documents et on est impressionné de voir ce que l'on a produit en une année. (je ne suis pas comme certains qui créent leurs billets de blog sur du word..).

Aussi, ma structure va évoluer vers une sauvegarde renforcée des documents du NAS (qui d'ailleurs est vieillissant niveau disque dur), et c'est là qu'est le drame chez Synology. Pas d'outils de backup générique pouvant s'interfacer avec owncloud, Mega....mais pour Box, si, à partir de DSM5 si mes souvenirs sont bons (l'outil existe depuis DSM4 je pense mais sans être très développé). Le passage par WebDAV ne me paraît pas très fiable, d'après les retours que j'en ai eu. Par contre, je peux très bien contourner le problème en mettant des règles de synchronisations sur un outil de backup d'un poste du réseau qui sera le poste maître. Si je l'ai testé sous windows, il me reste maintenant à le faire sur debian. Je n'ai pas besoin, par contre, de synchroniser des données entre terminaux, en dehors du calendrier et des contacts. La réflexion est donc en cours sur ce changement d'**outil de backup**. Enfin, il y a l'habitude à prendre sur le travail d'un document....

Si dans ma boîte, on a un document qui conserve toutes ses versions d'historique sur un serveur, c'est plus compliqué chez soi sur un NAS. La méthode "travailler localement" puis "sauvegarder en fin de session" sur le serveur, est une des possibilités. Ensuite, le décalage des backups de niveau 1 et 2 (respectivement un cloud et un disque dur) peut permettre de rattraper une erreur. Cela reste évidemment du bricolage mais le risque n'est pas non plus élevé. Autre technique possible : s'envoyer à soi même un mail avec le document, sur une boite sécurisée et archivée. A chacun de voir, encore une fois, si c'est un document très critique (mémoire de stage, roman, comptes personnels, documents d'une association...) ou pas. Il faut garder à l'esprit qu'il ne faut pas garder ses oeufs dans le même panier, donc ne pas avoir tout son "backup" dans un même emplacement physique/virtuel. Après, chacun trouvera des solutions avec, par exemple, des espaces serveurs chez un ami qui vous veut du bien, etc... A suivre.