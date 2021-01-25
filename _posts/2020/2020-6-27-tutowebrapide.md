---
layout: post
title: Tuto - Un web plus rapide, en vrai
category: tuto
tags: tutoriel, développement, geek, web, internet, hébergement, blog
---

**Je vous ai parlé du blog de backup que j’etais en train de monter…enfin c’est surtout les articles que je recopiais petit à petit, car la structure était là. Aujourd’hui c’est fini. Je milite depuis longtemps pour un retour à la simplicité, à la rapidité du web alors j’ai cherché à optimiser sans perdre trop au niveau de l’expérience utilisateur, c’est à dire en gardant des commentaires, de la recherche dans le site, par exemple.**

J’ai très vite cherché à faire un site statique puisque cela évite de recourir à une base de données, à trop d’outils externes. La logique était aussi d’avoir un fichier par article ce qui dans mon cas (plus de 1500 articles), représente une colossale base. J’avais aussi envie de faire du tri. J’ai donc cherché un truc qui me permette de transcrire une base wordpress xml en des fichiers les plus proches du texte, soit donc en markdown, ce langage à balise des plus simples. J’ai trouvé l’outil pour faire le passage en automatique grâce à ce développeur.

### Le Cahier des charges

Je ne voulais rien avoir en local, c’est à dire ne pas faire appel à du easyphp ou autre outil pour visualiser avant le site. Une fois le template présent, l’article doit s’insérer dedans. Je ne voulais que des fichiers sources en html, markdown et css, ce que j’arrive encore à comprendre facilement. J’ai découvert l’existence des githubpages qui permettent cela. J’ai fait un fork d’un template existant parmi les plus basiques et j’ai donc commencé à bosser dessus pour comprendre comment c’était fichu. Je préfère parti d’un truc qui fonctionne plutôt que de tout recréer de A à Z, je perds moins de temps. En plus cette base est suffisamment populaire pour trouver de la doc, malgré une absence de support depuis 3 ans. Oui, je prends un risque si évolution des githubpages et de ce qu’il y a derrière. Mais je pense pouvoir m’en sortir surtout qu’il reste encore des utilisateurs actifs.

### La solution choisie

Githubpages, c’est pas de pub, pas de coût d’hébergement dans mon cas puisque aucune image ou presque. Pas besoin d’installer jekyll en local, déjà que c’est une cata sous windows 10. Pas envie de faire subir ça non plus à ma Debian. J’attaque directement le code et je regarde des prévisualisations des pages markdown localement quand je les édite. Pour le peu de scripts en langage Liquid (natif sur jekyll ), ça peut se tester directement, github gère les version. Il a juste fallu que je pose un peu ma structure des catégories wordpress sur un papier pour le repenser pour ce site. J’ai environ 6 Mo d’articles en plus du peu de base qu’il y a pour le site. Ridicule. J’ai compris rapidement qu’il y aurait des manques :

* Pas de moteur de recherche
* Pas de nuage de tags et de menu par catégorie
* Pas de commentaires
* Pas de liaison vers des réseaux sociaux
* Pas de sitemap

J’ai cherché des solutions à ces problèmes. Pour le premier cas, il y a des possibilités d’intégrer des versions perso des moteurs de recherche comme duckducgo, google ou qwant. J’ai choisi ce dernier parce qu’il y avait facilité à le personnaliser par rapport à DDG. Par contre, pour l’instant les résultats sont pitoyables alors je redirige sur google (en rajoutant un paramètre !g dans le code ) le temps que la base de Qwant soit à jour…Hum je pense déjà à l’après vue la gouvernance de Qwant. La mise à jour, c’est lent, même chez les concurrents quand c’est quasi quotidien chez le géant américain.

Pour les commentaires, la base que j’utilise avait déjà prévu le coup en prenant Disqus. Et ça marche suffisamment bien pour ce que je veux en faire. Il suffit pour cela d’avoir un compte admin disqus. J’en avais gardé un depuis des lustres. En plus ça fait un lien vers des réseaux sociaux donc ça répond à mes deux problématiques.

Ah oui, le sitemap a l’air d’être intégré mais en fait ça ne fonctionnait pas terrible alors j’ai pris un script liquid pour ça que j’ai mis dans une page sitemap.html. Par contre le feed RSS fonctionne parfaitement sans rien touché et j’ai mis ça dans les icones du footer (le bas du fichier)

Les nuages de tags, bon, c’est sympa mais finalement c’est peu utilisé. Il manque vraiment les liens dans les tags des articles mais c’est tout. Pour les menus, j’ai utilisé du liquid pour des pages par catégorie. J’ai rangé ça dans un répertoire spécifique et j’ai mis un petit script qui me cherche tous les articles en regardant l’item « category » qui est déclaré en en-tête de chaque article. Ca me génère la page automatiquement. J’ai mis un « if » avec l’opérateur « contains » pour toute ce que je veux faire apparaître dans la page et j’ai même fait un petit menu en haut qui dirige vers des « ancres » pour chaque sous-partie de la page. Simple, efficace et rétro.

Je peux faire de même sur les tags de chonologie que j’ai intégré dans les articles pour faire la chronologie que je faisais à la main dans wordpress. Pour le nuage de tags, il pourrait y avoir une solution en sélectionnant avant des tags parmi les plus populaires mais finalement je n’en vois pas l’intérêt.

Enfin, il y a une limitation à 1000 fichiers par répertoire dans Github. c’est problématique pour un gros blog comme le mien. L’astuce est de faire des sous répertoires par année dans le répertoire _posts et tout fonctionne sans rien toucher puisqu’il regarde juste tout ce qu’il y a dans _posts pour construire le site.

Restait à tester **la rapidité de l’engin** et c’est assez édifiant. J’ai comparé avec mon ancien blog de backup sur une page perso free (pas connu pour sa vélocité)

Avec GT Metrix on a ça

![gt1](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2020/gtmetrixfree.jpg)

![gt2](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2020/gtmetricwp.jpg)

![gt3](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2020/gtmetrixgithub.jpg)


Avec Googe Insight Speed on a ça

![gis1](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2020/insightfree.jpg)

![gis2](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2020/insightwp.jpg)

![gis3](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2020/insightgh.jpg)

Avec Pingdom on a ça

![ping1](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2020/pingdomfree.jpg)

![ping2](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2020/pingdomwp.jpg)

![ping3](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2020/pingdomgh.jpg)

Les résultats se recoupent parfaitement sur les requests et les tailles de page. Je pensais avoir fait mieux en taille par mon choix de thème sur l’ancien backup mais c’est raté. Malgré la vélocité de worpress.com aujourd’hui, j’ai quand même du retard par rapport au temps de chargement. La taille est bien divisée par 10, donc c’est ce que je voulais. Les performances sont quasiment au max de ce que je pouvais faire. Les résultats du backup chez free sont aussi très parlants. Ce n’est pas fait pour ça maintenant et en plus Free est toujours 2 ans en retard sur les versions.

### Et après?

Maintenant la question qui se posera sera de savoir si un jour je passe définitivement sur ma solution github pages ou pas ? Il manque la partie programmation d’article évidemment qui est un grand confort sur wordpress, même par rapport à d’autres plateformes concurrentes. Les brouillons, ça peut se gérer encore en laissant des drafts par ailleurs dans une rubrique à part. Il manque surtout une facilité de création de liens entre articles par rapport à WordPress qui sait regarder directement dans sa propre base. Forcément, pas de base, pas de chocolat. Question forme c’est le plus épuré que je pouvais, pas au point d’un RMS et son fourre-tout, quand même. J’ai encore à retravailler quelques aspects de forme et de fond. Il faut aussi que je rajoute des commentaires sur les ajouts, même si j’en ai mis dans le readme. Tout ça se trouve ici : [le github](https://github.com/Icemanfr75/icemanfr75.github.io)

Par contre cette solution n’est pas du tout adaptée à une utilisation multi-compte avec plusieurs utilisateurs. C’est exclusivement pour des pages personnelles, des sites simples. C’est pour cela que pas mal de sites qui ont basculé sur cette solution sont revenus à … wordpress qui reste quand même le plus simple d’accès et le plus complet. On voit qu’avec le bon thème, les bonnes options et le bon hébergement, on arrive à de bons résultats. J’ai d’ailleurs profité de cela pour enlever le superflu de mon footer de ce site. Il y en a encore beaucoup, trop surement…Vous en pensez quoi ?
