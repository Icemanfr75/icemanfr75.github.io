---
layout: post
title: Tuto - Ajouter un bouton mastodon sur son blog Jekyll
category: tuto
tags: développement,jekyll,mastodon, github, pages
---

**Un site moderne ne peut plus se passer de boutons de partage. Il y a évidemment ceux des méchants réseaux sociaux dominants mais aussi ceux des réseaux alternatifs comme Mastodon. Sauf qu'il faut préserver la confidentialité des utilisateurs.**

Je suis parti d'un travail lu sur le [blog de Webjeda](https://blog.webjeda.com/share-buttons-jekyll/). Il y a donc un fichier share.html à rajouter dans les _includes de votre site d'abord. C'est la partie de code qui apparaîtra en bas de la page, enfin là où vous voudrez. Par rapport à la version d'origine, j'ai rajouté le titre de l'article dans ce qui est mis en automatique.

Code :

![code1](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2020/mastobutton1.png)

Ensuite, il faut rajouter justement ce petit code dans le fichier de _layout qui décrit les pages d'articles, c'est à dire post.html

Code :

 `include share.html` avec les habituels crochets et %

Enfin, il faut rajouter du code dans la feuille de style pour décrire le comportement, les couleurs,etc...

Code :

![code2](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2020/mastobutton2.png)

Me manquait alors mastodon, ainsi
J'y ai rajouté le même principe que ce que j'avais fait sur wordpress, c'est à dire un bouton sans JavaScript pour la confidentialité. Je fais en fait appel à [une page hébergée](https://sharetomastodon.github.io/about/) sur github et qui recense la plupart des instances mastodon. Il suffit juste d'adapter un peu le code et le rajouter à notre fichier share.html

Code :

![code3](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2020/mastobutton3.png)

Il n'y a plus qu'à reconstruire le site et remettre ça en ligne. 

Vous aurez remarqué que les images utilisées sont distantes. Il est possible de changer ça et de les héberger chez soi évidemment. Pour plus de facilité, vous trouverez le code sur [mon github](https://github.com/Icemanfr75/icemanfr75.github.io).
