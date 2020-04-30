---
layout: post
title: Tuto - Gérer ses photos gratuitement
category: tuto
tags: gestion, logiciel, photographie, tutoriel,
---
**Pour qui veut trier et organiser ses photos numériques, les solutions ne manquent pas. Mais derrière les poids lourds du marché Apple Aperture/Photo (sur Mac) et Adobe Lightroom, il y a des solutions gratuites. Oublions un instant Picasa de chez Google, devenu de plus en plus lourd et peu souple avec les NAS. ACDSee reste un produit payant. Alors que faire ?**

Il existe tout d'abord le logiciel <a title="XNView" href="http://www.xnview.com/">XNView</a> <a title="xnview" href="http://www.xnview.com/">,</a> disponible sur toutes les plateformes dans sa version beta baptisée MP ou sur Windows dans sa version normale. Léger, facilement configurable, avec des plugins, il permet l'essentiel : Editer les données EXIF et IPTC, classer, faire des retouches légères, et convertir éventuellement. Largement suffisant pour de la photographie non professionnelle, où le format RAW n'a pas vraiment d'utilité. Sa grande force est dans le traitement par lots pour le renommage, la conversion et l'édition de métadonnées. Il manque toutefois une fonction dans la version "normale", la géolocalisation des photos prises à posteriori.

Cela peut paraître gadget mais il est parfois agréable de fixer l'endroit où a été prise une photo. Sur des numérisations de diapos, des photos prises il y a quelques années, il faut avoir recours à des logiciels ou passer par des sites d'archivage. Autre possibilité, passer par <a title="Geosetter" href="http://www.geosetter.de/en">Geosetter</a> , qui utilise aussi les données EXIF, fait un peu de classement mais surtout utilise google maps pour trouver les coordonnées à inscrire en métadonnées. Malheureusement, il n'existe pas de version multiplateforme de ce logiciel allemand. La sélection par lot est très agréable également. Sous GNU Linux, il reste aussi possible d'utiliser <a title="DigiKAM" href="https://www.digikam.org/node/671">DigiKam</a> , produit dans l'environnement KDE.

Pour gérer ses photos sur un NAS, l'astuce est souvent de créer un "lecteur virtuel" en connectant le répertoire "photos" de son NAS, sous Windows. Sous GNU Linux, il suffit de monter le répertoire du NAS au démarrage dans un répertoire baptisé "photos" par exemple. La méthode et les fichiers à éditer peuvent varier selon les types de distributions mais il est évidemment conseillé de fixer l'adresse IP de son NAS dans son réseau local.

**Utilisation de XNView MP**

Si l'on se penche sur l'utilisation de ce logiciel, il faut bien comprendre certains points.

**Les différents types de Tags **

Pour bien comprendre le monde obscur des metadonnées liées aux fichiers photos, il faut savoir qu'il existe conjointement 3 formats de données. Les données EXIF sont inscrites par l'appareil photo à la création de l'image. Elles renseignent sur les conditions techniques de l'appareil (ouverture, vitesse, sensibilité, etc...) ainsi que sur la marque et le modèle du matériel. A cela s'ajoutent les 2 formats de Tags qui sont gérés par les logiciels : L'IPTC et le XMP. Pour être plus exact, on devrait parler d'IPTC-IIM pour information interchange model. C'est un standard utilisé par de nombreux types de fichier et qui s'est retrouvé vite limité. Le XMP en est le prolongement sous l'égide d'Adobe (Photoshop) et utilise un format XML intégré au fichier conteneur. Il peut rajouter donc de nombreuses balises/tags. Dans XNView, il est difficile de faire la différence entre l'IIM originel et le XMP mais on verra ensuite qu'il existe d'autres "mots clés". Dans Windows, l'onglet Détails des propriétés d'un fichier donne accès à ces données XMP.

**Comment les éditer**

<img class="alignnone size-medium wp-image-164" src="https://cheziceman.files.wordpress.com/2016/01/iptc-window.jpg?w=300" alt="iptc-window" width="300" height="156" />

Dans le mode "Browser" uniquement Un simple Ctrl+I ou un clic sur l'icone en forme d'étiquette amène une boite de dialogue. Il est possible de sélectionner plusieurs fichiers pour rajouter des mots clés identiques. <span style="color:#ff0000;">**Mais attention, il n'est pas possible de supprimer un même mot clé sur plusieurs fichiers**. C'est un problème général dans le monde de l'image où finalement il est préférable de vider ses mots clés et les recréer que tenter une suppression hasardeuse. En sélectionnant plusieurs fichier, le bouton &lt;Enregistrer&gt; sauve les modifications du fichier visualisé en vignette en haut à droite. On peut se déplacer dans la sélection avec les flèches en dessous. Le bouton &lt;Tout Enregistrer&gt; enregistre les modifications pour tous les fichiers. Attention, cela peut être très long sur des gros fichiers sur un lecteur réseau.

**Tags ou Catégories**

Lorsque XNView ouvre un répertoire dans le mode "browser" il met à jour son "Catalogue" avec des vignettes et les tags de chaque fichier. Il importe ces tags dans une catégorie "Autres" qui permet un affichage beaucoup plus rapide qu'une recherche. Mais la modification de ces catégories n'implique aucunement la modification des tags correspondants. Il faut réimporter le catalogue dans le fichier XMP (une fonction accessible dans le menu pour chaque sélection de fichier) en gardant à l'esprit que le logiciel ne fera que rajouter et ne remplacera pas. Il n'y aura donc aucune suppression des tags dont on a supprimé la catégorie équivalente. La synchronisation entre ces deux mondes n'est donc pas évidente. Je conseille de <span style="color:#ff0000;">**travailler d'abord sur ses métadatas et de refaire une mise à jour complète du catalogue** du répertoire concerné lorsque l'on a terminé.

**Notes et couleurs**

Il est possible de rajouter des données supplémentaires pour aider au tri. La première est la Note sur 5 étoiles. Par défaut, la note dans XNView est dissociée des métadatas XMP (les étoiles qui apparaissent dans windows par exemple). Pour que les deux soient liés, il faut aller dans les préférences du logiciel, rubrique metadonnées/metadata et cocher la case &lt;Exporter la note vers XMP&gt;. La deuxième donnée est une pastille de couleur à choisir encore entre 5 valeurs (Rouge, Orange, Bleu, Vert, Violet ). Si par défaut XNView a attribué des noms, il est possible de les changer et de faire ce que l'on veut. Là encore, la donnée peut être intégrée en XMP en cochant la case &lt;Exporter le libellé couleur vers XMP&gt;. dans les préférences. Il peut être par exemple intéressant de donner une couleur sur les fichiers que l'on souhaite retravailler ou bien encore ceux qui sont pour une utilisation professionnelle.

A noter que par rapport à XNView, son concurrent Picasa n'utilise pas toujours correctement les mots clés / tags et ne peut créer de notes ou de couleurs, se contentant de "favoris", une donnée illisible en dehors de Picasa. Là encore, il vaut mieux privilégier un standard ouvert et lisible par le plus grand nombre.

**Utilisation multi-utilisateur**

Lorsque l'on travaille sur un lecteur réseau comme un NAS par exemple, il convient d'abord de faire ses grosses retouches sur une image en local puis de la répercuter sur le réseau une fois terminé. Mais pour les tags et autres métadonnées, l'ajout et la suppression peut très bien se faire en distant, les données étant directement dans le fichier. Par contre, le catalogue et les catégories seront stockés sur le poste de consultation et ne seront mis à jour que sur action volontaire de l'utilisateur (par exemple l'ouverture d'un répertoire réseau).
