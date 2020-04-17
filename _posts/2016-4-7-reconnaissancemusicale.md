---
layout: post
title: Reconnaissance musicale - Les applis en test
category: geek, tutoriel
tags: android, geek, iOS, Musique, reconnaissance, Tutoriels
---
**Les smartphones d'aujourd'hui savent reconnaître des titres musicaux qui passent à la radio ou ailleurs. deux applications se partagent le marché, Shazam et Soundhound. Je rajouterai l'application native Sony sur mon Z1 Compact : Track ID**

Il faut savoir que lorsque l'on fait écouter un titre à ces applications, beaucoup d'autres données peuvent transiter en même temps. Cela fait partie du modèle économique et les permissions repérées par LBE Security Master sont légions. Pour que tout le monde soit sur un pied d'égalité, j'ai supprimé toutes les permissions sauf sur l'enregistrement sonore et le réseau de données. Les applications ont l'utilisation suivante de votre smartphone  :


* Shazam : 42,8Mo d'installation, 72Mo de mémoire, et 2,5% de CPU ....sur mon Snapdragon 810
* Soundhound : 38,4 Mo d'installation, 76Mo de mémoire et 1,5% de CPU
* TrackID : 26,6Mo d'installation, 29Mo de mémoire et 1,8% de CPU

Au niveau **ergonomie**, Shazam use et abuse des publicités et promotions de musiques. Soudhound est beaucoup plus sobre, se contentant de rappeler l'historique de recherche. On peut aussi regarder les tendances et une carte, comme pour Shazam. CHez TrackID, la carte trone en haut de l'interface, elle aussi très sobre.

<img class="alignnone" src="https://lh3.googleusercontent.com/9is_dcjmOwDgG9h9CFjFVVkwDpzbNPjiZ_NApHbcfJ0N32VJ3qToXl4cjgiFp7xOKQ=h900" alt="" width="507" height="900" />

Passons maintenant au **test de reconnaissance**. Evidemment, les titres à la mode sont reconnus, comme beaucoup de titres de Majors. Le but est plutôt d'aller chercher des vieilleries, des artistes peu connus. Le résultat est sans appel puisque seul Shazam a reconnu successivement Zoe Keating, Myrkur. Pour Myrath, ou Sanjay Leela Bhansali, c'est le statu quo entre les 3 applications. Pour un vieux Thierry Amiel, c'est Soundhound qui est le plus lent des 3 à trouver. Mais un des derniers single de Shakaponk a refusé obstinément d'être reconnu par TrackID. Plus étonnant encore est la reconnaissance sur des titres classique qui  va jusqu'à l'interprêtre. Cela marche très bien donc avec des émissions sur les radios classiques ou dans "vous avez dit classique" sur France Inter. Mais pas de miracle pour des domaines un peu moins "grand public", comme de la Country diffusée sur Musicbox radio, par exemple.

Au niveau de la "**puissance" du son** nécessaire, j'ai testé cela en réglant le son petit à petit au plus bas, jusqu'à ce qu'une application ne puisse rien détecter, sans bruit de fond et sans changement de positionnement par rapport à la source. A ce petit jeu, ex aequo pour Soundhound et Shazam avec un niveau sonore acceptable pour environ 30db mesuré au sonomètre (à comparer au bruit de fond de 18db). TrackID a bien du mal à faire le tri et se trompe même de titre.

En conclusion, on comprend pourquoi Shazam domine le marché, bénéficiant à la fois d'un avantage technologique, mais aussi d'une base de données bien plus importante. On paye cela par une lourdeur et une intrusivité abusive du produit. Le challenger reste toujours Soundhoud, TrackID fermant la marche avec bien peu d'atouts, sinon sa légèreté. Il faut bien avouer que l'on utilise pas cela tous les jours. Et si vous comptez siffler un morceau pour qu'il soit reconnu, c'est encore raté !

