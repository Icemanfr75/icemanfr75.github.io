---
layout: post
title: Tuto mobile - Bien utiliser le web- 1, les liens
category: tuto
tags: bonnes pratiques, internet, mobile, tutoriel, 
---
**Les liens sont au coeur de l'internet mais notre regard est aujourd'hui attiré ailleurs. Ils apportent à la fois une aide, mais peuvent aussi révéler des pièges. Comment bien naviguer à l'heure de l'internet mobile.**

Dans l'internet dit "fixe" (sur ordinateur), avec un large écran, l'internaute disposait de beaucoup d'informations et de confort pour utiliser son navigateur correctement. Aujourd'hui, beaucoup découvrent ce média à travers leur smartphone et/ou une tablette, ce qui, même avec un très grand écran, ne permet pas de voir tout ce qui se passer derrière. Je vous propose ici d'avoir quelques bons réflexes.

**Notions techniques**

Je sais qu'il est toujours chiant de commencer par de la technique mais ce n'est pas toujours barbant et ça aide à comprendre ce que l'on fait ensuite. Car il faut savoir ce qu'est **une page web**, déjà. Il s'agit d'une suite de codes, un programme qui va décrire ce qui sera affiché à l'écran et indique où se trouve chaque élément source. Pour le traduire on va utiliser **le navigateur,** un logiciel capable de comprendre et de retranscrire à l'écran ce code. Dans ce code, on fait appelle à plusieurs langages, à des sous programmes (en java, en flash, par exemple) qui vont parfois demander l'installation de petits logiciels (des extension ou plugins) mais qui sont de plus en plus intégrés dans le navigateur, surtout sur mobile. Mais on parle surtout de navigateur car chaque "page", est localisé par son adresse, un truc en http://www.adresse.xx ou même sans le www aujourd'hui. Il y en a aussi d'autres types (ftp://ftp.stockage.xx par exemple...), mais je vais m'arrêter là.

Cette adresse en réalité est une suite de chiffres, qu'on appelle **adresse IP,** mais que des serveurs savent traduire en noms plus facile à retenir. Pour faciliter la mémorisation de tout cela, on a créé des **favoris ou bookmarks,** sorte de petit carnet d'adresse personnel pour sauvegarder les sites que l'on veut reconsulter. Autrefois localisés sur l'ordinateur, ils sont aujourd'hui sauvegardés à distance avec le profil utilisateur, notamment sur smartphone...Mais je suis obligé de parler aussi des types de navigateurs. D'origine, il y a Safari coté Apple et Chrome coté Google Android. Je conseille plutôt<a href="https://cheziceman.wordpress.com/2017/05/12/tuto-naviguer-mobile-et-libre-avec-moins-de-publicites/"> Firefox pour Android</a> pour des raisons de confidentialité, de liberté que vous allez comprendre ensuite. Il y en a d'autres (dont Opera, UC Browser, Dolphin Browser, Liberty Browser ...) qui ont des avantages ergonomiques ou techniques. L'un d'eux, aujourd'hui courant, est l'utilisation d'onglets mais qui peut se présenter de différentes manières. Voyons l'exemple de Chrome :

<img class="size-medium wp-image-20296 alignnone" src="https://cheziceman.files.wordpress.com/2017/05/chrome1.png?w=169" alt="" width="169" height="300" /><img class="size-medium wp-image-20297 alignnone" src="https://cheziceman.files.wordpress.com/2017/05/chrome2.png?w=169" alt="" width="169" height="300" />

Puis celui de Firefox :

<img class="alignnone size-medium wp-image-20298" src="https://cheziceman.files.wordpress.com/2017/05/firefox1.png?w=169" alt="" width="169" height="300" /><img class="alignnone size-medium wp-image-20299" src="https://cheziceman.files.wordpress.com/2017/05/firefox2.png?w=169" alt="" width="169" height="300" />

Dans les deux navigateurs, on a :

* La barre d'adresse ou de recherche
* La gestion des onglets qui donne accès à ...
* Le rajout d'un onglet
* Un premier onglet ouvert
* Un deuxième onglet ouvert

Petit bonus pour Firefox qui donne accès très facilement au mode "privé" (6), c'est à dire avec moins de traces, pas de cookies, etc...

**Le Choix du navigateur .... et du moteur de recherche**

Pour la plupart des personnes, Recherche = Google (ou Siri). Mais j'ai déjà expliqué <a href="https://cheziceman.wordpress.com/2017/01/08/blog-lillusion-de-la-realite/">le danger </a>de ne faire confiance qu'à un seul moteur de recherche. Donc on peut penser utiliser Duck Duck Go, Qwant, .... Mais pour que ce soit simple, il faut que la recherche consiste à taper des mots dans la barre d'adresse en haut et de lancer sa recherche. Problème : Aucun navigateur actuel ne permet de **choisir librement son moteur de recherche**... sauf Firefox. Tous les autres ont une liste limitée et non modifiable, basée sur des contrats avec des géants du web (Bing pour Microsoft, Yahoo pour... ce qu'il en reste, Google pour Alphabet, et j'ai quasiment fait le tour).

Après, j'ai parlé d'ajouts. L'un des ajouts indispensable aujourd'hui est le "**filtre antipub**". Indispensable car comme je l'ai expliqué, une page web fait appel à des sous-programmes, des scripts, qui vont ouvrir d'autres pages ou parties de pages non désirées par l'utilisateur avec parfois des effets néfastes (pompage de données utilisateur, blocage....). Les navigateurs mobiles intègrent des filtres antipopup mais rarement un filtre aussi efficace que µBlock origin. Seul Firefox Android/iOS permet son intégration (Liberty Browser n'est pas assez mûr selon moi). Voici comment le faire : <a href="https://cheziceman.wordpress.com/2017/05/12/tuto-naviguer-mobile-et-libre-avec-moins-de-publicites/">Tuto</a>

Vous voilà enfin prêt à la découverte de l'internet d'aujourd'hui.

**Et les liens dans tout ça**

Contrairement à un pc classique ou le passage de la souris sur une zone permet de voir le lien s'afficher l'adresse dans la barre d'état (aujourd'hui c'est une petite zone qui apparaît en bas à gauche de l'écran), sur un mobile, on ne peut prévoir ce qui va se passer en cliquant sur une zone de l'écran. Donc **DANGER.** Ils peuvent ainsi déclencher une publicité (via un script), une ouverture d'image, de vidéo ou pire, d'un programme malveillant. Mais ne sombrons pas non plus dans la paranoia. Car les liens sont placés dans différents secteurs de la page :

* Dans le corps du texte, vous voyez des éléments soulignés et dans des couleurs pouvant aller du <span style="color:#0000ff;"><u>bleu</u> au <span style="color:#ff0000;"><u>rouge</u> en passant par le<span style="color:#000000;"><u> noir</u>.
* Dans des boutons ou zones d'images ressemblant à des boutons de commande
* Dans des photos ou captures de vidéos
* Dans une zone de la page où il n'y a rien.

Pour les deux derniers cas, c'est évidemment très sournois et le réflexe à avoir est de fermer tout de suite cet onglet....et de fuire la page, si ce n'était pas votre volonté d'aller voir cela. Pour les autres, on peut avoir quelques autres réflexes :

* Ouvrir dans un nouvel onglet. Ca évite toujours de bloquer / perdre la page que l'on consultait. Pour cela, **l'appui long est votre ami.** Il fait apparaître un menu contextuel en général. On peut même l'ouvrir en mode privé.
* Copier le lien et le coller ensuite pour regarder si l'adresse n'est pas suspecte. C'est un peu lourd, c'est vrai...
* Mais le meilleur réflexe et de ne pas fréquenter des sites douteux (sexe, piratage, ventes de produits interdits ...) et de se méfier des zones de publicité des sites d'information.

Voilà pour les premiers bon réflexes à assimiler. A suivre.
