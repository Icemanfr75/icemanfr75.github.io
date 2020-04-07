---
layout: post
title: Tuto - Switcher sous Linux Etape 2 - Les premiers tests
category: tuto
tags: distribution, linux, logiciel libre, tutoriel, tuto
---
**Après avoir défini son choix sur une distribution Linux, il reste à vérifier que tout sera bien pris en compte avant l'installation complète. Pour cela, voyons un peu le principe des Live CD et l'exemple de la Fedora dans sa release 14.**

Le fonctionnement que je vais décrire est quasiment valable pour toutes les distributions disposant de LiveCD. Un live CD c'est un CD bootable, c'est à dire que l'on insère au démarage de la machine pour qu'il se lance à la place du disque dur habituel. Il faut évidemment avoir activé l'option dans le bios de la machine, ce qui est maintenant souvent le cas. Les Live CD se récupèrent sous forme d'archive ISO gravable par n'importe quel logiciel de gravure. Il faut juste choisir le type de processeur et ....l'environnement graphique.

Encore une fois, je ne vais pas m'attarder sur toutes les possibilités d'environnement graphique qu'offrent les distributions car elles sont quasi infinies. Il faut juste savoir que pour l'utilisateur, il s'agit de l'aspect des fenêtres et boutons, des accessoires fournis. Bref, c'est un peu comme si on choisissait ce que l'on voulait voir comme type de fenêtre dans son windows et les accessoires qui vont s'installer. Cela ne paraît rien mais ce choix va avoir un impact sur les installations des logiciels par la suite. Je vais restreindre le choix aux deux environnements majeurs :
* KDE : A l'origine, il s'agit du portage linux d'un environnement pro Unix, CDE, avant d'évoluer rapidement vers une ergonomie plus proche de Windows. C'est l'environnement sans doute le plus répandu et qui a permis une vulgarisation de Linux. Il comprend aussi des bibliothèques et API pour les programmeurs et beaucoup d'outils dont KOffice, une suite bureautique.
* Gnome : C'est le concurrent et l'outsider. Il est resté plus sobre que son concurrent et un peu moins développé question API et bibliothèques. Une question de goût donc mais aussi d'intégration à la distribution choisie.

Vous avez choisi? Alors après avoir gravé le CD, il ne reste plus qu'à le mettre dans le lecteur et relancer le PC. C''est évidemment plus long que sur un disque dur et après quelques minutes, on arrive devant une boite de dialogue en environnement graphique si tout se passe bien. Désolé, je ne vais pas traiter des problèmes de reconnaissance à ce niveau mais si cela se passe mal, je conseillerai de chercher une autre distribution plutôt que de s'obstiner à vouloir installer celle là...surtout pour un débutant.

Si vous êtes arrivé à ce stade, c'est forcément que vous cherchez un avantage à linux : le prix, vouloir le stricte nécessaire, la performance, l'attirance vers le logiciel libre? Il y a de multiples raisons pas forcément toutes compatibles. Lors du test de ce live CD, il faudra voir s'il répond à votre attente. Pour l'instant il faut vous connecter sous ce live CD non personnalisé et en explorer les possibilités. Premier écueil : faire reconnaître son matériel et ses périphériques.

Vous risquez d'avoir un clavier en Qwerty. Il faut donc aller faire un tour dans le panneau de configuration ou les propriétés du système pour régler le langage. Ensuite il y a la résolution de l'écran : et hop, les propriétés graphiques. Est-ce que la carte graphique est parfaitement reconnue? Là, c'est plus dur à savoir avec les options 3D des cartes récentes. Mais si vous êtes sous Linux, ce n'est pas vraiment pour jouer car les derniers jeux PC ne sortent pas sous Linux, même si on verra qu'il y a des possibilités. Et le réseau, internet? Là, c'est obligatoire de l'avoir et il faut que sa carte réseau ou sa clé Wifi soit reconnue. Ce n'est pas plus compliqué que sous votre Windows ou votre OSX maintenant si le matériel est reconnu...ou plutôt c'est aussi peu simple pour le débutant. Si ce n'est pas reconnu, je réédite mon conseil au débutant : essayez en un autre.

Je sais qu'il y a des moyens de faire reconnaître son matériel, que les forums et sites d'aide sont nombreux mais sans réseau, il faut jongler entre 2 pc ou deux systèmes sans arrêt ce qui va prendre beaucoup de temps et décourager le débutant. D'où mon conseil de tester autre chose.

L'imprimante, le scanner? Alors là, il va falloir chercher un peu plus, surtout si le matériel est récent. Les constructeurs ne pensant pas à Linux, il faut se rabattre sur des pilotes génériques qui ne prendront pas forcément en compte toutes les fonctions de vos périphériques. Votre Smartphone? Avec un peu de chance, vous pourrez "monter" le téléphone comme un disque externe. Monter?? qu'est ce que c'est que ça?

Avec Linux, il va y avoir quelques notions de vocabulaire à apprendre :
* Monter : c'est rendre accessible des données par le système. Un CD que l'on insère, un disque dur formaté Windows, un disque externe, une clé USB....si on les mets dans Windows, après quelques instants, ils sont accessibles directement dans l'explorateur. Pas forcément dans Linux et il faut les "monter", du nom de la commande Mount sous Unix. Rassurez vous, certains périphériques montent automatiquement sur les versions récentes et orientées grand public mais parfois il va falloir jouer de la ligne de commande.
* Root : c'est le nom que l'on donne au super utilisateur qui peut rajouter des logiciels, configurer des paramètres du système, etc.... Il est déconseillé de travailler en Root par défaut pour éviter les mauvaises manipulations.
* Terminal : c'est l'équivalent de la fenêtre DOS de Windows, où on saisit des lignes de commandes. Elle est encore très utile dans un linux malgré les outils en mode graphique.

ça y est, vous avez trouvé le bon live CD pour votre matériel? Alors voyons maintenant les applications disponibles....Elles sont souvent accessibles par un menu équivalent au ménu démarrer de Windows ou bien un lanceur ou dock comme OSX. Découvrons les ensemble dans la suite....


