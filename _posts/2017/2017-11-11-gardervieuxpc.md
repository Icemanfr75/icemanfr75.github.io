---
layout: post
title: Blog - Quand il faut encore garder les vieux... PC
category: geek
tags: geek, Geekeries, informatique, mesure, recherche, technologie
---
**Avec le progrès, on te fait vite jeter ton Windows XP, voir Seven, ton GNU/Linux 32 bits, ton Pentium monocoeur, ton disque dur à plateaux, ton écran cathodique. Bon, c'est vrai que chez moi, je comprends sans tomber complètement dans le piège. Mais il y a des domaines d'activité où on ne peut tout simplement pas...**

Heureusement que je ne travaille pas dans le <a href="http://www.tomshardware.fr/articles/processeur-espace-CPU-NASA,5-199.html">spatial</a>, car là, c'est pire. Dans les satellites, on utilise de vieux processeurs et des matériels très largement éprouvés, évidemment dans des versions particulières, mais aussi parce qu'on fait appel à des technologies et programmations anciennes. Mais sans aller jusque là, il suffit de travailler avec des matériels de mesure ou des matériels électroniques pour constater le problème. J'avais déjà parler de la généralisation des <a href="https://cheziceman.wordpress.com/2017/02/10/tutoscience-comment-les-fabricants-de-materiels-sadaptent-a-la-fin-de-lhegemonie-windows/">microserveurs</a> pour configurer le matériel. Mais l'argent se faisant rare dans les entreprises, on recycle du vieux matériel, on ne renouvelle pas tout et on se retrouve alors avec un matériel qui ne se gère qu'en RS232, alias port série. Vous savez, c'est le truc à 9 broches qu'on avait avant sur les PC... remplacé par l'USB aujourd'hui.

<img class="aligncenter size-medium wp-image-21538" src="https://cheziceman.files.wordpress.com/2017/11/9_pin.jpg?w=300" alt="" width="300" height="130">

Pas grave, me direz vous, il suffit de mettre un convertisseur RS232/USB; il y en a des tonnes sur le marché et ça coute presque rien. Avec ça, tu te récupères un bon vieux clone d<a href="https://fr.wikipedia.org/wiki/HyperTerminal">'hyperterminal</a> et&nbsp; tu peux envoyer tes instructions, récupérer une trame d'information , etc... Un bon vieux câble croisé à 4 ou 5 fils (voir même 3 pour le txd, rxd et masse par exemple) suffit souvent pour faire la liaison. Je me commande à distance une balance de pesée par exemple, pour pouvoir intervenir dans un banc en fonctionnement sans me mettre en danger. Mais après on a plus compliqué : J'ai eu dans l'idée d'utiliser un générateur arbitraire de chez Agilent (ex Hewlett Packard instrumentation, aujourd'hui Keysight), un truc qui peut te balancer n'importe quel signal électrique de faible tension sur 80MHz et pas seulement des sinus ou triangles comme les générateurs habituels. Le truc vaut aujourd'hui près de 3500 Euros, sachant qu'il est abandonné depuis 2016 et ça a plus de 15 ans, facile. Agilent oblige, tu as du GPIB (IEE488), du RS232 et par contre pour ce dernier, tu as besoin des 9 fils pour communiquer en cable dit Null Modem.

<img class="aligncenter size-medium wp-image-21537" src="https://cheziceman.files.wordpress.com/2017/11/33250a.png?w=300" alt="" width="300" height="165">

**On va faire un peu technique, là**.... Mon objectif était de reprendre un signal enregistré et de le modifier pour le "rejouer" à l'aide de ce générateur. Je ne vous dirai pas pourquoi, je devrais vous tuer après... Pour ça j'ai donc besoin d'un logiciel pour créer ma forme d'onde et l'envoyer ensuite sur le matériel. J'ai le logiciel d'époque, à peine remis à jour mais il lui faut une bibliothèque d'entrées/sorties (IO Library en anglais). Je télécharge la bibliothèque 2017 : ça se passe mal avec le proxy de ma boite. Je prends la version 2014, ça passe et je lui rajoute un pilote à la main. J'installe mon logiciel (gratuit) et là .... rien, il ne voit pas le matériel alors que les utilitaires de la bibliothèque semblent les voir après le réglage de la vitesse , du bit de parité, du nombre de bits dans la trame. ...Ok, je vois que je vous ennuie. Alors j'installe la version d'essai du nouveau logiciel sensé remplacer l'ancien. C'est une usine à gaz de 500Mo qui au final me permet juste de faire...On/Off (Il en faut 200 de plus pour définir une forme d'onde) mais refuse obstinément de me balancer ma programmation en entier. Le problème semble dans la vitesse de transfert et la taille du buffer/tampon car le RS232 c'est lent....En réalité, c'est une fonction, le Handshake, qui ne passe pas avec le convertisseur RS232/USB. Je l'ai appris quand après 2 jours d'essais, j'ai fait appel au support. Il m'aurait fallu passer par le GPIB...ça vaut 700 Euros le cable, plus 720 Euros de licence du nouveau logiciel ! Papa noel n'est pas passé.

![tuto](https://cheziceman.files.wordpress.com/2017/11/kusb.jpg)

*Si quelqu'un veut me faire un cadeau...*

**And now ... the solution !** Alors j'ai eu l'idée de ressortir un vieux PC doté d'un port série, d'un vieux XP et qui me sert uniquement à programmer des vieux clous. Me voilà à trouver la vieille version de la bibliothèque, heureusement disponible chez le constructeur, avec le vieux logiciel derrière et j'ai tout installé en 3/4 heures sur le vieux disque dur bruyant de cette tour Pentium II. Miracle, en l'espace de 5 minutes, je faisais ce que j'essayais de faire depuis 2 jours. Je peux très bien programmer mon signal confortablement sur mon portable, sauver le fichier et le transférer ensuite sur ce pc pour programmer mon générateur. La virtualisation et les convertisseurs ne servent à rien mais tout ça vient aussi de l'aspect propriétaire de ces matériels que l'on a du mal à piloter par des solutions plus "libres". J'en ai vu essayer de piloter ça par des programmes variés, c'est la galère et de toute façon, il te faut la bibliothèque d'entrées/sorties.

![tuto2](https://cheziceman.files.wordpress.com/2017/11/handshake.gif)

*Formats de handshaking*

Moralité, on a tout intérêt à toujours se garder un vieux PC dans un coin, les sauvegardes des logiciels qui vont avec, les câbles (on a du recâbler le Null Modem nous même) car il arrive un jour où les vieilles interfaces ne sont plus supportées, où l'on laisse tomber le 32 bits, etc. Mais attention à ne pas garder cet ordinateur branché sur un réseau, à ne pas échanger des fichiers avec d'autres n'importe comment car évidemment, c'est le genre de PC qui sera la première victime, faute de support. On l'a vu dans le médical, autre domaine fauché comme les blés, où des services arrêtaient de travailler faute de machine opérationnelle. Car dans mon cas, si je réutilise ce matériel, c'est aussi parce qu'un plus récent est utilisé sur un autre projet. Et qui sait si justement dans 10 ans on n'utilisera pas tous un produit conçu grâce à ce générateur et ce PC préhistorique, sans le savoir? Évidemment, le fond du problème est dans l'investissement qui se fait rare dans nos industries, tout autant que dans les abandons prématurés de support ou bien dans des développement logiciels baclés ou pas adaptés à l'utilisation réelle (il faut voir leur "suite" avec la gestion des licences en plus pour le croire... en plus il n'y a rien de prévu pour gérer via un proxy). Tout ça pour dire que tous les "dinosaures" ne doivent pas disparaître!

[la video](https://www.youtube.com/watch?v=vgiDcJi534Y)

ps : ne me remerciez pas pour ce titre qui vous trottera dans la tête aujourd'hui...