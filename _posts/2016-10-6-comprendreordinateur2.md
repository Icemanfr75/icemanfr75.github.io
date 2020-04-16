---
layout: post
title: Comprendre son... Ordinateur - Vol.2
category: tuto
tags: geek, informatique, ordinateur, pc, tutoriel,
---
**Après un premier article présentant l'architecture et le fonctionnement global de l'ordinateur, allons un peu plus loin. Parlons de pannes courantes.**

**Mon logiciel "plante"**

Le symptôme est classique. Alors que tout semble se passer correctement, le logiciel que l'on utilise disparait soudainement de l'écran sans prévenir...ou bien après un message d'insulte incompréhensible. Avouons le, c'est le cas le plus complexe à solutionner car il y a une infinité de possibilités. Si cela arrive alors que le Système d'Exploitation (ou OS pour Operating System, voir épisode précédent) vient d'être démarré, et que cela fonctionnait correctement il y a quelques jours, c'est probablement qu'un élément, auquel fait appel le logiciel pour fonctionner, a été détérioré. Éventuellement, la **désinstallation puis la réinstallation **(soit lui redonner les bases de son métier et du langage) du logiciel peut régler le problème. Mais si cela arrive après d'autres utilisations logicielles, cela peut aussi être du à ce que l'on appel "**un conflit mémoire**" : La mémoire vive ou RAM de l'ordinateur est utilisée en créant des "petites cases" ou adresses. Un peu comme si pour classer les dossiers en cours sur notre bureau, nous nous étions fait une étagère avec plein de numéros pour se souvenir où se trouve quoi. Mais parfois, on se trompe et on veut mettre un dossier dans une case déjà remplie. Et là, ça bloque. Le problème est qu'à cause de cela, on ne peut traiter le dossier en cours et qu'en plus on ne sait pas qui a mis l'autre dans cette case. La seule possibilité est d'essayer de reproduire l'incident en lançant successivement un des autres logiciels puis celui qui a planté. Et si cela se reproduit, il faudra probablement choisir de se passer d'un des deux ou là encore de les réinstaller, voir de les mettre à jour dans une autre version. Mais il n'y a pas toujours de solution.

**L'ordinateur met du temps à réagir**

Et soudain **l'écran se fige** ou les actions de l'utilisateur n'ont plus de conséquence. La tentation est évidemment de tout arrêter à l'aide du bouton marche-arrêt. Car derrière ce figeage ou gel, il peut y avoir différents problèmes. Là encore, c'est vraisemblablement un problème de mémoire mais qui peut aussi bien venir de l'OS que d'un logiciel. Pour comprendre ce qui se passe, le réflexe est encore d'essayer de reproduire la situation en enchainant les dernières actions réalisées avant ce gel. Mais parfois le gel est temporaire et du uniquement à un "trop plein" d'information à gérer. Son autre manifestation est le fameux ...

**L'Ecran bleu Windows**

Il s'agit d'une manifestation d'un arrêt du bon fonctionnement du systéme d'exploitation. J'ai choisi de parler de l'écran bleu de Windows car c'est d'une part le système d'exploitation le plus courant, mais c'est aussi devenu un symbole, depuis Win95/98. Les messages s'inscrivant sur cet écran sont rarement déchiffrables par un débutant et pourtant il y a souvent l'indication d'une erreur (error) sur un fichier, voir d'un conflit mémoire (memory). L'anglais est votre ami. J'avoue ne pas avoir rencontré de telles erreurs sur un système d'exploitation autre, que ce soit OSX ou Debian, donc je ne ferais aucun parallèle. La solution est de noter sur un bout de papier le message (forcément, pas de copie d'écran possible), de tenter de redémarrer, de chercher ensuite ce que vous avez noté dans un moteur de recherche et là, peut être comprendrez vous. Mais il faut aussi se souvenir de l'action que vous faisiez juste avant. Il se peut justement que ce soit suite au fonctionnement d'un ou deux programmes successivement ou conjointement.

Reste aussi une autre hypothèse à ces ralentissements : Les virus et autres <span style="text-decoration:underline;"><a href="https://fr.wikipedia.org/wiki/Logiciel_malveillant">Malwares</a>. Solution: mettre à jour votre antivirus, passer un programme d'antimalware comme celui malwarebytes, par exemple...

**L'Ecran noir au démarrage**


Il peut apparaître à plusieurs moment. Si vous ne voyez même pas l'écran de démarrage de l'OS ou même pire le BIOS, alors le symptome est probablement Hardware (écran, carte graphique, barette mémoire, voir pire). S'il s'accompagne de bips, alors c'est même sur. Si c'est après la mire du système d'exploitation, il est possible qu'un composant soit déterioré. Dans ce cas, le premier réflexe (sous windows en tout cas) est de savoir si ça se reproduit en mode sans échec. Un appui sur la touche F8 pendant le démarrage permet d'y accéder.  Si la machine démarre, youpi, vous aurez peut être la possibilité de la réstaurer. Sinon, il restera la possibilité de booter sur un CD de réinstallation, ou de tout réinstaller. Cela peut être aussi du à un problème de disque dur car si un composant est déterioré, c'est parfois à cause du disque dur qui a perdu la donnée. Dans ce cas, après le redémarrage (mode sans échec ou pas), pensez à sauvegarder vos données importantes sur un support externe.

**le Bip qui fait peur**

C'est le bip long qui vient au démarrage ou pendant le fonctionnement, la série de bip avant les symptomes vus avant. Et si c'est ça, c'est un défaut hardware donc du matériel. Ca peut être une surchauffe (vérifiez si le portable ne chauffe pas, si les ventilateurs ne sont pas obstrués, s'ils tournent encore....). Pour un PC fixe, on peut démonter et changer des pièces pour tester (si on en a). Pour un portable, c'est beaucoup plus compliqué. Pour savoir si c'est une surchauffe, faites un redémarage immédiat et regardez si le bip apparaît rapidement. Arrêtez le PC 1/4h et redémarrez aussi et regardez le temps qui passe. Eventuellement, faites tourner la même application que vous utilisiez au moment du premier bip. Le type d'application peut orienter vers le problème. Mais la case "spécialiste" risque d'être indispensable à moins d'avoir une collection de pièces détachées.

Malheureusement, on voit qu'il y a beaucoup d'hypothèses à balayer à chaque fois dans ces cas, autant au niveau du matériel que du logiciel. Un point de sauvegarde régulier et des sauvegardes de vos fichiers permettent de palier au plus urgent et de ne pas être trop géné dans votre travail. Pensez, surtout sous Windows, à mettre à jour antivirus et produits de sécurité.

A suivre...
