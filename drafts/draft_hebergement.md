---
layout: post
title: Réflexion - le retour de l'hébergement ?
category: reflexion
tags:  
---
[status draft]

**Cela fait plus d'un an que j'ai entamé une réflexion sur le support du blog. Wordpress est très bien et pratique mais de plus en plus lourd à gérer à force de vouloir tout faire. Entre auto-hébergement, hébergement ou sous-traitance complète, mon coeur balance toujours.**

Le matériel m'a pas mal forcé à **changer la façon de "produire" des articles**. Maintenant je le fais complètement en mode texte brut et je les partage sur un espace à moi tant que ce n'est pas finalisé. Je ne compte jamais les versions mais elles sont nombreuses. Ce n'est peut-être pas le plus pratique par rapport à l'interface wordpress, mais c'est efficace. Wordpress, c'est sympa mais lorsque j'ai repris l'ensemble des articles, j'ai retrouvé au moins 4 types de codage et c'est bordélique. Si j'ai arrêté de gérer moi même un site wordpress (il y en avait une copie jusqu'en Juillet hébergé ailleurs), c'est justement pour ne plus être emmerdé avec les versions, les évolutions de plugins qui créent des failles. Un choix qui se "paye" par des incursions publicitaires et des cookies de stats, etc...Et puis, malgré un travail sur la forme pour alléger au maximum, le site est encore un peu trop lent à mon goût dans mon optique de rendre le web rapide à nouveau. Je me tape en plus des googlefonts et un tas de trucs que je voudrais virer. Bosser sur du texte brut rentre donc dans cette logique, bien loin des blocs qui ne remplacent pas un bon vieux copier coller si rapide avec quelques raccourcis clavier.

Ce soucis de revenir aux basiques s'est d'abord traduit en 2020 par **la mise en place d'une github page** avec donc un template très léger, des fichiers markdown qui correspondent à chaque article et qui permettent la "reconstruction" du site à chaque ajout ou mise à jour. Le problème vient que ça se base sur Jekyll qui utilise ruby comme langage, avec un peu de liquid sur les pages en plus du markdown. Ruby est lourd à installer et on se retrouve à être prisonnier de ce langage, de ses évolutions, etc. Sur windows, j'ai trouvé ça lourd. Sur debian, je m'en suis démerdé avec la vieille debian à l'époque mais c'était long sur ma vieille machine à reconstruire le site. Si bien que j'ai tapé directement dans l'interface web de github pour mettre toutes les pages. 1400 articles à refaire, avec quelques automatisations mais au moins un code à peu près homogène. Si je passe à autre chose, le markdown a l'avantage d'être reconnu partout ou presque. Mais donc je ne veux pas être prisonnier de ce langage, de cette plateforme et j'ai imaginé autre chose : Pour résumer, chercher le langage le plus universel et simple à installer partout pour transformer mes fichiers markdown en du html que je n'aurai plus qu'à exporter sur le serveur ensuite. D'une idée simple, on tombe vite dans le compliqué. Avec le temps, je me dis que les tags ne servent à rien d'autre qu'aux moteurs de recherche, que les commentaires, ça peut se faire autrement (disqus, mail) et que les catégories, ça peut s'afficher dans des pages archives comme je l'avais fait avec mes scripts liquid.


Il se trouve que l'ami [F6K](http://shl.huld.re/~f6k/log/) a parlé d'autres personnes qui sont aussi dans cette même optique ou ont des solutions à eux pour cela. Je recherche la simplicité et la robustesse en faisant cela, chose que Wordpress ne m'apporte qu'au prix d'être chez eux. Ma démarche est extrème mais instructive pour moi. Alors j'en ai regardé des exemples. J'ai regardé les principaux moteurs de sites statiques et ça ne me plait pas car on s'enferme à nouveau dans autre chose. J'ai regardé d'autres blogs, imaginer des formes comme j'ai trouvé par exemple chez [Karl Dubost](https://www.la-grange.net). J'ai vu leurs difficultés, les écueils et continué à chercher mon Graal. J'ai testé 11ty, aussi mais si le système paraît ouvert, je trouve que Node.js reste un problème comme je l'ai évoqué plus haut. Python pourrait être la solution car relativement courant aujourd'hui. 



comment j'imagine

les problèmes rencontrés

le coût par rapport au gain

d'abord le nom de domaine, un cout raisonnable.

ensuite l'hébergeur qui ne fera pas faillite, ne fera pas n'importe quoi
J'oublierai free puisque peu à peu ljélimine toute dépendance Abul FAI 

la programmation d'article impossible,  la consrvation des brouillons
