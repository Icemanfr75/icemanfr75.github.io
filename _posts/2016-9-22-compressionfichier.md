---
layout: post
title: Tuto - La Compression pour les nuls
category: tuto
tags: tutoriel, compression, transfert
---
**La compression de fichier paraît souvent complexe pour bien des utilisateurs, alors que parfois ils manipulent des fichiers déjà compressés, sans le savoir. Voilà l'occasion de faire un point sur les bons usages.**

**Les origines et les formats**

Il fut un temps où les utilisateurs d'ordinateurs n'avaient pas Internet pour s'échanger des fichiers et passaient par des disquettes. Et comme ces données sont en réalité une succession de 0 ou de 1, des petits malins se sont dit qu'il y avait sans doute de la place à récupérer dans tous ces fichiers et qu'il fallait trouver un moyen de compresser, tronçonner et recoller les fichiers pour les placer sur des disquettes. Je ne vais parler dans un premier temps que des formats de compression SANS pertes, c'est à dire qu'on veut à l'arrivée un fichier de la même qualité que celui de départ.

<img class="alignnone size-full wp-image-1726" src="https://cheziceman.files.wordpress.com/2016/08/msdoszip.jpg" alt="msdoszip" width="533" height="138" />

Je vous passe les détails des algorithmes de <a href="https://fr.wikipedia.org/wiki/Codage_de_Huffman"><span style="text-decoration:underline;">codage de Huffman</a>, qui date de 1952, et qui reste à la base de beaucoup de formats de compression, ou encore des LZ77, LZ78, .... Tous ces algorithmes ont donné naissance à une pléthore de combinaisons très proches les unes des autres, mais aussi incompatibles, chacun se disputant la palme de la plus forte compression. Les utilisateurs d'Unix et GNU Linux connaissent les formats TAR, GZIP, GZ,  tandis que ceux de Windows ont connu le ZIP, ainsi que ses principaux concurrents RAR, ARC ARJ et LZH (un peu moins à la mode), le plus récents 7Z, le ACE, et les utilisateurs de Mac connaissent aussi le SIT, et les fans de Microsoft connaissent le CAB. Tous ces formats regroupent dans ce qu'on appelle une Archive, un ou plusieurs fichiers de formats variés et avec un "taux de compression" variable (le rapport entre la taille du fichier compressé par rapport à la taille du fichier de départ).  Ce dossier n'est lisible que si on utilise le logiciel d'archivage approprié et qui affichera un dossier très comparable à ce qu'on retrouve dans une fenêtre de Windows/Debian/MacOS.... Enfin ça, c'est maintenant car autrefois, il fallait passer par de la ligne de commande en DOS/UNIX et de longs temps de compression avant d'obtenir le résultat souhaité.

**Choisir ses armes**

Je parlais du fait de mettre le fichier sur des disquettes. En effet, les programmes ont bien vite ajouté l'option de couper les fichiers en morceaux de la taille d'une disquette standard. le ZIP et son pendant WinZIP a fait longtemps fortune sur cette fonctionnalité bien pratique. Aujourd'hui, on fixerait plutôt la taille d'un CD ou du maximum qu'un site de partage puisse héberger, soit 650Mo ou 1Go, à la place de 640ko ou 1,4Mo. Mais ça c'est la création.... Le problème est de choisir un format qui sera compréhensible du destinataire et donc il faut connaître souvent son système d'exploitation (Windows, OSX, GNU Linux...) ou bien les outils dont ils disposent. Le premier réflexe est donc bien de s'entendre sur le format de partage ou bien alors d'indiquer comment l'utiliser. Aujourd'hui, sous Windows, le Zip est pris en charge directement par le système mais entretient un flou dans l'utilisation. On a l'impression que les fichiers contenus sont des fichiers d'un dossier. Sous Android, il faut avoir recours à une application, tandis que Gmail crée parfois une archive en ZIP lors de l'envoi de plusieurs fichiers. Bref, le ZIP est assez courant, tandis que chez les pirates, le RAR a souvent eu les préférences dans les échanges.

<img class="size-full wp-image-1727 alignleft" src="https://cheziceman.files.wordpress.com/2016/08/winzip.jpg" alt="winzip" width="316" height="435" />

Ces deux formats savent gérer les archives à fichiers multiples, qu'il faut laisser souvent numérotés avec la même racine du nom (par exemple nomfichier.r01 nomfichier.r02, etc...). Il suffit alors d'ouvrir un des fichiers pour que le programme ouvre aussi les autres et décompresse avec le bouton "Extraire"/"Extract".

**En avant la Musique**

La musique a été révolutionnée par le numérique et un format : Le MP3 ou Mpeg audio layer 3, créé par un institut allemand en 1992. Alors qu'avant un fichier de musique faisait 45Mo, il a permis de le réduire par 10 et donc de faciliter les échanges au temps où nous n'avions que des modems 56k. Napster le fera passer à la posterité. Mais contrairement aux autres formats vus auparavant, il s'agit d'un format destructif, détruisant ce que l'oreille humaine n'est pas sensée entendre. Il convient, selon moi, d'avoir au moins un bitrate de 192kbits/s pour maintenir un son correct, et plus surement 320kbits/s, ce qui crée des fichiers environ 5 à 6 fois moins gros qu'un format CD. D'autres formats permettent de maintenir une bonne qualité tout en étant compressés : Le OGG Vorbis, format proche du monde du libre, et le AAC bien connu des fans d'Apple et d'iTunes. Je ne parlerai pas ici du problème des DRM (digital right management ou gestion des droits), ni du WMA de Microsoft, qui tend à disparaître. En format quasi non destructif, on a aussi le format FLAC, très prisé des audiophiles mais qui nécessite vraiment de bonnes oreilles et un bon casque pour faire la différence avec du OGG de bonne qualité. On retrouve aussi des archives ZIP/RAR contenant des fichiers MP3 ou FLAC, ce qui du point de vue compression n'a pas de sens. Mais il est plus facile de télécharger un seul fichier que 10, donc dans ce cas la compression ne sert qu'à réunir des fichiers.

**Et pour les yeux ?**

Tout possesseur d'appareil photo numérique utilise la compression sans même sans apercevoir. En dehors des pros qui utilisent les formats dits RAW, le commun des mortels utilise le JPEG qui est un format destructif. Les fabricants d'appareil photos tentent de trouver le meilleur compromis taille/qualité mais il y a quelques pertes qui se voient souvent dans le lissage excessif de l'image, ou bien dans des pixelisations. L'utilisateur a parfois la possibilité de régler le "taux de compression" mais il vaut mieux garder plus de 80% de qualité. En dehors de la photo numérique, on peut aussi trouver d'autres formats qui permettent de gagner de la place par rapport au BitMap (BMP) de base. On peut ainsi utiliser le PNG, remplaçant du GIF (limité à 256 couleurs et sous brevet), ou le TIFF qui ne précise pas le type de compression qui se trouve derrière car il s'agit d'un Conteneur.

<img class="wp-image-1728 size-full" src="https://cheziceman.files.wordpress.com/2016/08/jpegcomp.jpg" alt="jpegcomp" width="648" height="431" />
Un JPEG trop compressé (source Harvard)

**Le problème du Conteneur**

<img class="size-full wp-image-1730" src="https://cheziceman.files.wordpress.com/2016/08/mkv.jpg" alt="Un outil de création de MKV" width="549" height="284" />
Un outil de création de MKV

Le <span style="text-decoration:underline;"><a href="https://fr.wikipedia.org/wiki/Conteneur_vid%C3%A9o">conteneur</a> est un format de fichier qui ne précise pas quel est le type de compression incluse. l'AVI en est un bon exemple puisqu'on peut avoir une vidéo AVI non compressée, une autre en compression DivX, une autre en XVID, en AAC vidéo, en H264.... Selon la présence d'un <span style="text-decoration:underline;"><a href="https://fr.wikipedia.org/wiki/Codec">CODEC</a> sur la machine, on pourra ou non le lire. Dans le monde de la vidéo internet, on connait aussi le fameux MKV, possédant l'avantage de garder plusieurs pistes de sous-titres. Plus rare est le WebM de Google, prévu pour la diffusion de vidéo sur internet. Et sur smartphone, on connait le 3GP. Il faut aller voir dans les informations du fichier pour voir le nom du compresseur utilisé et donc pouvoir le lire. Un programme comme VLC (présent sur toutes les plateformes) permet de lire la plupart de ces fichiers conteneurs. Quant à la création de ces fichiers, il faudrait un tutoriel complet pour en parler au niveau vidéo, tant il y a d'options.

**Les documents bureautiques et leurs pièges.**

L'erreur du débutant dans la création de documents bureautiques (autant Word que Write), est d'insérer des photos issues directement de fichiers JPEG haute définition. Sauf que lors de cette insertion, le traitement de texte reconvertit l'image dans un format non compressé (Bitmap) et la taille du fichier texte résultant est énorme. A ce moment là, l'utilisateur va probablement compresser son fichier en Zip pour le transférer au destinataire (ou bien d'abord créer un PDF....qui sera aussi trop gros) alors qu'il faudrait utiliser une fonction bien pratique du traitement de texte : La compression d'image. Par exemple, sous Word, ça donne ça :

<img class="size-full wp-image-1732 alignleft" src="https://cheziceman.files.wordpress.com/2016/08/wordcomp.jpg" alt="wordcomp" width="504" height="327" />

* Aller dans l'onglet Outils d'image, Format, Ajuster et cliquer sur l'icone "compresser".
* Vous aurez alors différentes options de "sortie cible" qui correspondent non pas à une simple compression, mais à un changement de résolution d'image (d'où les chiffres en ppp pour point par pouce)
* Pensez alors à la destination du document, sachant qu'en passant en PDF, la transformation reprendra aussi les réglages du document texte d'origine.
* Attention aussi aux copier-coller de tableaux issus d'un tableur (Excel, Calc...) qui prennent parfois tous les onglets du document et pas seulement la zone sélectionnée. Cela peut être très génant lorsqu'il y a des données confidentielles sur les autres onglets cachés. Il faut faire un "Collage Spécial" et utiliser "conserver la mise en forme source".

**Les échanges de fichiers et leurs dangers**

Pour éviter de se faire repérer, les personnes qui échangent des fichiers mp3 ou xvid utilisent parfois des archives. Mais comme on ne voit pas tout ce qu'il y a dedans au premier abord, on peut aussi télécharger des virus, scripts malveillants. Alors avant de décompresser, vérifiez toujours avec un antivirus à jour et ne faites pas de décompression "à la volée" avec le bouton droit / extraire ici. Il vaut mieux ouvrir le fichier en lecture avec l'outil de décompression, sélectionner les fichiers voulus et cliquer sur extraire en ne prenant pas les fichiers superflus. D'autres utilisent parfois une fausse extension. Le fichier n'est pas un .bmp de 650Mo mais en réalité un . rar qu'il faudra renommer avant de l'extraire. Là aussi, attention aux faux amis. Mais de toute façon, vous savez que pirater, c'est mal ;-)
