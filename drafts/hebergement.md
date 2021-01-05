---
layout: post
title: Réflexion - Hébergement ou gamberge ?
category: reflexion, geek
tags:  hébergement, développement, site, web, réflexion 
---

**Cela fait plus d'un an que j'ai entamé une réflexion sur le support du blog. Wordpress est très bien et pratique mais de plus en plus lourd à gérer à force de vouloir tout faire (sans parler des incohérences créées par l'application mobile). Entre auto-hébergement, hébergement ou sous-traitance complète, j'ai tout fait et pourtant mon coeur balance toujours. Ca va être un peu technique...**

Le matériel m'a pas mal forcé à **changer la façon de "produire" des articles**. Maintenant je le fais complètement en mode texte brut / markdown et je les partage sur un espace à moi tant que ce n'est pas finalisé. Je ne compte jamais les versions mais elles sont nombreuses. Ce n'est peut-être pas le plus pratique par rapport à l'interface wordpress, mais c'est efficace. Wordpress, c'est sympa mais lorsque j'ai repris l'ensemble des articles, j'ai retrouvé au moins 4 types de codage et c'est bordèlique. Si j'ai arrêté de gérer moi même un site wordpress (il y en avait une copie jusqu'en Juillet hébergé ailleurs), c'est justement pour ne plus être ennuyé avec les versions, les évolutions de plugins qui créent des failles, des incohérences, le avec ou sans jetpack, etc. Un choix qui se "paye" par des incursions publicitaires et des cookies de stats, etc...Et puis, malgré un travail sur la forme pour allèger au maximum, le site est encore un peu trop lent à mon goût dans mon optique de rendre le web (le mien :p) rapide à nouveau. Je me tape en plus des googlefonts et un tas de trucs que je voudrais virer (javascripts notamment). Bosser sur du texte brut rentre donc dans cette logique, bien loin des blocs qui ne remplacent pas un bon vieux copier-coller si rapide avec quelques raccourcis clavier. En vieillissant, je travaille de plus en plus à "l'ancienne", avec des outils simples et efficaces.

![slowweb](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2021/hebergement2.jpeg)

Ce souci de revenir aux basiques s'est d'abord traduit en 2020 par **la mise en place d'une github page** avec donc un template très léger, des fichiers markdown qui correspondent à chaque article et qui permettent la "reconstruction" du site à chaque ajout ou mise à jour. Le problème vient que ça se base sur Jekyll qui utilise ruby comme langage, avec un peu de liquid sur les pages en plus du markdown. Ruby est lourd à installer et on se retrouve à être prisonnier de ce langage, de ses évolutions, etc. Sur windows, j'ai trouvé ça encore pire à installer mais finalement j'ai contourné l'obstacle en attaquant directement github...et en oubliant windows. Sur debian, je m'en suis démerdé avec la vieille debian de l'époque mais c'était long sur ma vieille machine à reconstruire le site. Si bien que j'ai tapé directement dans l'interface web de github pour mettre toutes les pages. 1400 articles à refaire, avec quelques automatisations mais au moins un code à peu près homogène, durant l'été 2020. Si je passe à autre chose, le markdown a l'avantage d'être reconnu partout ou presque, au détail de l'en-tête jekyll en yaml. Mais donc je ne veux pas être prisonnier d'un langage, de cette plateforme et j'ai imaginé autre chose : N'avoir que des fichier markdown .md à mettre en ligne. Mais cela n'est pas raisonnable pour plusieurs raisons.

Un **site statique**, puisqu'il faut appeler un chat un chat, c'est un ensemble de pages html, une feuille de style, un template, et une structure de fichier qui va avec. Pour passer des articles au site, il faut un générateur de site qui peut être local ou sur un serveur. Lorsque c'est sur un serveur, c'est considéré comme un site statique hybride, car s'il n'y a pas de base de données, il y a tout de même un langage, une interface genre "CMS". L'exemple que je connais c'est PluXML que [j'ai utilisé un an](https://icemanfr75.github.io/pluxml/) avant de revenir sur wordpress. Mon problème avec ça reste la dépendance à un développeur, les failles de sécurité pour accéder au CMS (idem wordpress), les mises à jour qui parfois mettent le bordel dans les plugins. En plus si c'est du php derriere, ca veut dire aussi bonne version de php. Sans plugins, vous me direz, ça peut le faire. Mais les templates ne sont pas des plus clairs pour moi, encore que depuis j'ai progressé. Dans le même genre, on a yellow ou même media wiki. Si je fais du local, le problème (comme pour Jekyll), c'est le langage derrière. Le Ruby, le Go (Hugo), le Vue, voire le javascript, ce n'est pas ma tasse de thé. Le python, ça pourrait se faire, car c'est devenu généralisé. Le problème est que derrière, on rustine aussi avec des ajouts via PIP (installeur de package python), et qu'il y a encore à gérer les évolutions des versions. Ca peut se faire et se gérer. Pelican aussi c'est du python mais là encore ça devient trop pour moi. J'ai l'impression de ne pas maîtriser ce qu'il se passe.

Donc j'ai trouvé **une base simple** (oui, je pars souvent du plus simple, ce qui explique pourquoi l'évolution de debian m'inquiète...on y reviendra une autre fois) que je comprends et peut faire évoluer : Makesite.py, développée par [une indienne](https://github.com/sunainapai/makesite). Son idée a été reprise par bien d'autres, dérivée ou copiée avec inspiration. J'en suis arrivé à un autre developpeur français qui tient un [blog](https://blogduyax.madyanne.fr) sur ce type de format (un peu différent) ainsi qu'une [autre variante](https://github.com/fspaolo/maksite) du même principe. Il a rajouté beaucoup de choses, dont une gestion des commentaires en statique via le mail. Ce qui rajoute aussi des dépendances mais c'est intéressant pour comprendre. Je ne ferai pas comme [Stéphane Bortzmeyer](https://www.bortzmeyer.org/blog-implementation.html) avec sa solution en XML, par contre, même si cela reste dans cet esprit... Il se trouve que l'ami [F6K](http://shl.huld.re/~f6k/log/) a parlé d'autres personnes qui sont aussi dans cette même optique ou ont des solutions à elles pour cela. Plusieurs cerveaux valent mieux qu'un, surtout quand ils sont mieux cablés pour ça que le mien. Nous avons exploré conjointement des solutions, des exemples et c'est toujours intéressant de confronter les points de vue.

Toute cette réflexion m'a fait aussi **réévaluer les besoins**, simplifier encore et encore. J'ai passé le site actuel (jekyll et wordpress) à la moulinette SEO pour comprendre aussi la mode actuelle, les oublis, les failles, sans pour autant céder à cela. D'une idée simple, on tombe vite dans le compliqué. Avec le temps, je me dis que les tags ne servent à rien d'autre qu'aux moteurs de recherche, que les commentaires, ça peut se faire autrement (disqus, mail) et que les catégories, ça peut s'afficher dans des pages archives comme je l'avais fait avec mes scripts liquid sur la version github. Ma démarche est extrême mais instructive pour moi. Alors j'en ai regardé des exemples. J'ai regardé les principaux moteurs de sites statiques et ça ne me plait pas car on s'enferme á nouveau dans autre chose. J'ai regardé d'autres blogs, imaginer des formes comme j'ai trouvé par exemple chez [Karl Dubost](https://www.la-grange.net). J'ai vu leurs difficultés, les écueils et continué à chercher mon Graal. J'ai testé 11ty, aussi mais si le système paraît ouvert, je trouve que Node.js reste un problème comme je l'ai évoqué plus haut. Ah oui, j'ai oublié de parler de Publii, de l'hybride offline...Un logiciel à installer ce qui rend encore plus prisonnier mais est orienté débutant. Pas vraiment pour moi. 

Si la situation de ma github page est fiable et légère, c'est **l'évolution de la plateforme** qui m'inquiète (tout comme wordpress). Vu le propriétaire (Microsoft...), je peux imaginer le pire. D'où la recherche d'une porte de sortie, qui peut aussi être chez le concurrent Gitlab, Framagit en transition... Aujourd'hui, je suis capable de faire un article de n'importe quel terminal du moment que j'accède à un moment à un éditeur de texte. Pas de programmation d'article par contre comme du temps de wordpress. Mais tant que wordpress.com dure, je le conserve quand même. Wordpress peut transcrire le markdown en théorie mais j'ai remarqué que ça fonctionne une fois sur deux avec les bugs actuels de ce foutu gutenberg. On peut même lui envoyer un article directement par mail, là encore avec le mode draft/brouillon reconnu plus ou moins. Pas besoin non plus d'envisager d'autres formats ou navigateurs comme en parlait [Ploum récemment](https://ploum.net/gemini-le-protocole-du-slow-web/). Je suis dans une sorte d'esprit KISS (pas le groupe! Keep It Simple, Stupid) pour le blog, au fond. Le Gemini me paraît lui même une mauvaise idée car on ajoute encore un protocole quand on pourrait faire plus simple en réunissant ce qui existe déjà : protocoles sécurisés, interprétation d'un langage balise comme markdown directement dans le navigateur. Lisez la FAQ de gemini, les justifications de leur choix sont bancales. Je rêverai que Mozilla soit prescripteur, mais bon. Là encore, c'est toute la gouvernance des standards du web qui pose question, aux mains des GAFAM. 

![gemini](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2021/hebergement1.png)

Et puis il y a **l'hébergement et l'adresse**. Pas sur que [icemanfr75.github.io](https://icemanfr75.github.io) soit la meilleure adresse. Reprendre un nom de domaine pour le reste des temps, pourquoi pas? Je pourrais même orienter selon des sous domaines sur les deux versions. Ca ne me coûterait que moins de 10 euros par an, pour l'instant, mais pour quoi, au fond? Cette question ne cesse de me tarauder. Quel gain j'en tirerai puisque j'ai suffisamment de lecteurs à mon goût tel quel. L'hébergement moi même sur wordpress, pas envie d'y replonger non plus et le coût sera bien plus important. J'ai quand même regardé les hébergeurs fiables, mais les propositions techniques sont des plus opaques quand on rentre dans le détail. Déformation professionnelle, j'aime rentrer dans le détail pour comprendre le nombre d'adresse, les certificats ssl, le DNSSEC, le débit, les connexions simultanées, etc... Toutes ces occasions de vendre des options ou de ne pas permettre certains usages. Je pourrais en profiter pour faire mon nextcloud (ce qui n'est pas possible partout) et des tas d'autres choses mais franchement, je n'ai plus envie de m'ennuyer à ça à mon âge avec les cinglés qui peuplent le réseau aujourd'hui. Il suffirait qu'un billet ne plaise pas pour qu'on me flingue tout, non merci. Parano, vous croyez? J'en ai vu être ennuyés pour moins que cela. 

Comme en plus j'ai viré mes adresses free et pages qui vont avec, **on oublie** aussi la solution de l'hébergement gratos, puisqu'en plus ça ne suit pas bien sur les versions, la fiabilité. Voilà ce qui a donc occupé mon cerveau quelques temps et continue régulièrement. La solution, il n'y a finalement que moi pour la trouver car il y a beaucoup de choix. Avouons qu'aujourd'hui, il n'a jamais été aussi simple de faire un site à soi, de l'héberger. Mais il n'a jamais été aussi compliqué de faire simple. Faire simple pour qui d'ailleurs, puisque la plupart des utilisateurs sont habitués à avoir des images qui bougent dans un navigateur. Quand je pense que j'ai débuté en tapant du HTML à la pogne et en créant les menus en frame, sans les feuilles de style. Autres temps... A croire que la simplicité se mérite et je me demande finalement si je ne vais pas continuer comme maintenant et attendre d'avoir franchement le temps de me pencher sur les scripts python que j'ai vu, de savoir gérer ces p.....ns de librairies supplémentaires sur tous les OS. La clé me semble justement dans la conversion markdown avec plusieurs possibilités. Me demandez pas pourquoi, la liberté est trop compliquée. Trois exemples, trois convertisseurs différents. Et toi lecteur, si je te demande ton avis, tu vas me répondre par...oups, des commentaires, bien sûr. Comme quoi c'est utile. Une chose est sûre, je ne recréerai plus jamais de forums, sauf si ce sont des animaux qui le fréquentent.  Allez, à mon prochain changement d'avis sur le sujet.

ps : quand je vous dis que c'est compliqué dans ma tête...

Bande son : [Zazie - J'envoie Valser](https://www.youtube.com/watch?v=mYBI34quHdM)