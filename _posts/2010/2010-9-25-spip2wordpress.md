---
layout: post
title: Tuto  - Wordpress, Spip, Dotclear et migration
category: tuto
tags: dotclear, migration, spip, tutoriel, tuto, wordpress
---
**Abordons un peu de technique pour les webmaster et bloggeurs à travers la vie de ce blog et la migration d'un autre site entre 3 CMS ou moteurs de sites et blogs.**

(tuto créé à l'époque où ce site était à une autre adresse en Wordpress...)

A l'origine, ce blog était sous **Dotclear** 1.x mais devant l'inertie de ce système, j'ai décidé de passer à **Wordpress**, alors en version 1.x également. L'interface du blog était assez sommaire et minimaliste tandis que le tableau d'admin comprenait tout ce qu'il fallait. Après une période de sommeil, j'ai fait la mise à jour en Wordpress 2.x pour en découvrir les nombreuses évolutions.

L'interface y est plus clair, avec de nombreuses possibilités et surtout la possibilité d'ajouter des plugins. Il est permis d'intervenir dans la mise en page et la config des templates directement sans passer par un logiciel de ftp et un éditeur texte. J'en ai donc été très satisfait. Parallèlement à ce blog, j'ai créé une page perso pour les tests de plugins, de templates, de design et de moteurs de site.

Mon autre site a été créé en **Spip** 1.x il y a 3 ans. J'avais choisi ce format car il ma paraissait plus adapté à un webzine et qu'on le rencontrait couramment dans des sites francophones comme Agoravox par exemple. Plutôt simple à installer, j'ai vite trouvé les limites du systèmes vis à vis de la mise en page. S'il reste possible de faire des templates évolués, il n'est pas pratique de les éditer. Après un basculement il y a un an en version 2.x de Spip, j'ai accueilli avec bonheur la possibilité de mettre des plugins et notamment un qui permet l'édition des fichiers directement au coeur de l'interface d'admin spip. Sauf que les stats du site ne sont guère fiables et qu'il reste peu évident de modifier le design pour le rendre vraiment moderne.

J'ai donc décider cette année de migrer sur Wordpress et tant qu'à faire, sur sa version 3.0.x, la dernière en date. Après pas mal de recherche pour trouver un moyen de conserver mes 120 articles avec photos dans cette migration, j'ai trouvé la solution <a title="Teklib" href="http://www.teklib.net/migrer-de-spip-vers-wordpress" target="_blank">ici</a>. Entre temps je me suis interessé à Drupal et Joomla mais l'ampleur du travail et l'impossibilité de trouver un outil de migration m'a fait laisser tomber cette solution. Si ces outils sont performants, ils sont trop complexes à mettre en place pour un simple Webzine.

Avec cette solution, il est nécessaire de passer par un site en dotclear. Me voilà donc à créer un site dotclear sur ma page free de développement. Attention, il faut utiliser postgreSQL et non mySQL pour Dotclear chez Free. Pas de souci car il est possible d'avoir les deux moteurs sql pour le même compte. Je pouvais donc avoir les deux sites Wordpress 3.x et Dotclear dans sa version 2.2. L'examen de cette dernière version de Dotclear m'a permis de constater qu'il conserve une longueur de retard sur Wordpress mais reste tout à fait performant face à un spip pour un blog ou même un Webzine assez simple. Restait donc à faire un backup de spip vers Dotclear, remettre un peu en forme les catégories et mots clés puis faire un backup vers ce site Wordpress de travail.

A ce moment, le site existait donc sur spip sur son adresse et sur la page de travail en Wordpress. Il n'y avait que les photos qui n'étaient pas sur Wordpress mais toujours sur la page "spip". En une demi heure, il a été possible ensuite d'installer un wordpress sur la page spip, de supprimer la base sql de spip, de récupérer la base Wordpress de la page de travail grace aux fonctions d'import/export. Ensuite, comme je n'avais que 120 articles et d'autres ajouts à faire, j'ai passé un peu de temps à remettre les images dans la structure de wordpress à la place de celle de Spip. Avec le recul, j'aurai pu tenter de faire autrement en attaquant directement la base SQL et les liens d'image qui y sont inscrit. Il ne restait plus qu'à supprimer le répertoire des images de Spip.

Avec cette méthode, le site n'a connu quasiment aucun arrêt. Le seul problème vient du changement d'adresse des articles et chroniques et on perd donc un peu en fréquentation. Mais les gains sont importants :

	* Designs modernes et facilement modifiables
	* Intégrations de réseaux sociaux
	* Intégration plus facile de médias audios et videos
	* Gestion de plusieurs utilisateurs autant que Spip

Me voilà donc avec un site et un blog à gérer sous une interface similaire, ce qui est un gain de temps certain. Attention également aux mises à jour des extensions qui peuvent bugger. Il est conseillé de tester d'abord sur la page de travail avant de le déployer sur le site définitif.
