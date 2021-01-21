---
layout: post
title: Tuto/test - Le meilleur player musical Android
category: tuto, geek
tags: android, flac, Geekeries, mp3, Musique, ogg, player, test
---
**Depuis l'abandon de l'appli Walkman/musique sur mon Sony Z1Compact, j'étais à la recherche du player musical ultime, que ça soit pour un petit téléphone comme le Moto E, ou un truc plus large comme mon actuel Xiaomi Redmi 4A. Je suis exigeant aussi coté son et je ne veux pas perdre en fonctionnalités.**

### Mon cahier des charges

...est exigeant bien qu'assez classique:

* Jouer du MP3, du Ogg, du Flac
* Savoir gérer une playlist ou une liste de lecture
* Jouer dans l'ordre défini par l'album et utiliser les tags essentiels que sont artiste et nom de l'album
* Savoir faire du repeat one, du repeat all
* Avoir un son puissant et détaché (une bonne dynamique)
* Être léger à l'utilisation et sur le téléphone (idéalement moins de 30Mo)
* Avoir un timer/minuteur pour l'extinction
* Avoir un widget de petite taille
* Ne pas avoir de pub
* Être gratuit

Vous noterez que je ne parle pas de formats HD, d'utilisation de convertisseurs analogiques numériques USB, etc... Pour ça, il faut oublier le smartphone et une utilisation nomade, même avec un très bon casque. Je m'en suis remis à un Sennheiser PX100, un Koss PortaPro et mon intra Novodio habituel. Pour les fichiers audios, j'ai utilisé des Flac et Ogg de l'album de <a href="https://cheziceman.wordpress.com/2015/05/08/zoe-keating-into-the-trees/">Zoe Keating</a> et d<a href="https://cheziceman.wordpress.com/2017/03/19/musique-akira-kosemura-momentary/">'Akira Kosemura</a>. Enfin, j'ai fait quelques enregistrements avec un "sonomètre" de smartphone et un analyseur de spectre, des instruments qui restent évidemment tributaires de la réponse en fréquence du microphone de l'engin. Ce n'est donc qu'en relatif les uns par rapport aux autres qu'il faut regarder ces mesures en complément de l'oreille humaine.

Après avoir testé plus d'une vingtaine de produits, je m'en suis remis **aux players suivants** :

* <a href="https://play.google.com/store/apps/details?id=com.kodarkooperativet.blackplayerfree">Blackplayer</a> : souvent cité par les sites de référence, hum.... très sensibles au sponsoring.
* <a href="https://play.google.com/store/apps/details?id=com.rhmsoft.pulsar">Pulsar</a> : Bien vu sur XDA...dans sa version gratuite (pas d'égaliseur)
* <a href="https://play.google.com/store/apps/details?id=in.krosbits.musicolet">Musicolet</a> : Le plus léger dans les players modernes
* <a href="https://f-droid.org/packages/com.android.music/">Player Android</a> de base (celui disponible sur F-Droid) : Il manque des choses mais c'est une référence encore aujourd'hui
* <a href="https://play.google.com/store/apps/details?id=com.hiby.music">HibyMusic</a> : Orienté qualité et HD
* <a href="https://f-droid.org/packages/ch.blinkenlights.android.vanilla/">Vanilla Music</a> (aussi sur F-Droid): Libre et plein de fonctionnalités

Pas de PlayerPro, N7Player ou Poweramp qui sont des produits trop lourds et payants. Pas de foobar ou AIMP dont l'ergonomie est vraiment trop bizarre pour un utilisateur normal. Evidemment, pas de PlayMusic ou d'ITunes non plus.

### Taille des applications

Les applications ont été installées puis lancées avec scan de la bibliothèque puis arrétée.

* Blackplayer : 29,3 Mo
* Pulsar : 17,4 Mo
* Musicolet : 13 Mo
* Player Android   : 1,6 Mo
* HibyMusic : 91,3 Mo
* Vanilla Music : 2,4 Mo à l'installation mais 3,59 après premier démarrage

**Fonctionnalités**

![image](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2017/fonctionplayer.jpg)

Au regard de l'attendu, nous avons déjà deux grands gagnants qui sont **Pulsar** et **Musicolet** (**10/10**). Pour **Vanilla** **(7/10)** et **Black player (9/10)**, l'accès au timer est malaisé . A noter aussi que **Hiby** **(6/10)** et Vanilla créent leur propre bibliothèque musicale au premier démarrage, en dehors de l'indexation d'Android. Et évidemment, j'ai eu des soucis de réactualisation avec Vanilla. L'**Android player** n'a qu'un manque : le minuteur. (**8/10**)

### Interface

* **Blackplayer** : L'interface est moderne mais sombre (forcément). Il y a beaucoup d'options de tri pour la playlist mais ça pollue l'écran. On utilise beaucoup le slide pour accéder aux fonctions ou changer de piste. Il faut valider d'abord l'accès au minuteur dans le menu général qui est peu accessible et le minuteur n'est pas directement accessible en mode lecture. **6/10**
* **Pulsar** : Une interface classique et claire. La gestion de la playlist peut parfois avoir des bugs même si le suivi est régulier. Il est trop facile de faire glisser les titres par mégarde. L'égaliseur est en option.** 8/10**
* **Musicolet** : Le look est austère avec beaucoup de boutons pour la gestion de la playlist qui est très évoluée. Beaucoup d'accès directs comme le minuteur mais par contre le repeat fait appel à un sous-menu. **6/10**
* **Player Android **  : Interface très démodée et austère mais fonctionnelle. Il manque évidemment des fonctions mais tout y est pour juste écouter de la musique et retrouver ses fichiers. **6/10**
* **HibyMusic** : L'ordre est peu gérable pour la playlist. Beaucoup de boutons peu compréhensibles. Mais il y a un bouton quitter.** 5/10**
* **Vanilla Music** : Material design pour les artistes. le timer est seulement configurable dans les paramètres. Des fonctions de normalisation du son sont implémentées. **7/10**

### Qualité sonore

C'est l'application Sonomètre et l'application Spectroid qui ont été utilisées. La première sur un extrait musical pour noter le max et la moyenne de son produit, et la seconde sur un autre extrait pour regarder la dynamique et la finesse. Attention, les valeurs en dB n'ont pas de signification absolue.

![image](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2017/playertest.png)

* **Blackplayer** : Une bonne définition et une amplitude importante mais des saturations marquées dans les medium. **6/10**
* **Pulsar** : Une bonne définition et une dynamique assez faible pour un son fin **6/10**
* **Musicolet** : Une dynamique importante et une définition peu nette qui donne parfois un sentiment d'étouffement. **4/10**
* **Player Android**  : Une bonne définition mais une amplitude faible. Un son assez consensuel **6/10**
* **HibyMusic** : Un son moins dynamique mais plus fin et détaché qui évite des saturation, notamment dans les basses **8/10**
* **Vanilla Music** : Un son très peu défini avec trop de dynamique. On voit des saturations à certaines fréquences. Un son flatteur mais trompeur **4/10**

Avec ces extraits de spectromètre, on repère quelques tendances à la saturation et des basses très marquées, notamment chez Vanilla et Black Player. Ce dernier a tout de même un son bien détaché dans les aigus où Pulsar pèche parfois tandis qu'Hiby nécessite d'être un peu plus poussé que les autres. Bien évidemment, je n'ai pas utilisé les égaliseurs internes.

![image](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2017/image4663.png)

### Conclusion

![image](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2017/notesplayer1.jpg)

Il n'y a aucun choix parfait. Mon préféré reste Pulsar pour son homogénéité et son ergonomie . Le player Android reste, malgré son austérité, un bon choix homogène, surtout pour de vieux smartphones. Blackplayer mériterait un meilleur son et des améliorations d'interface. Avec un très bon casque et dans un bon environnement, on pourrait justifier Hiby mais ça n'a strictement aucun intérêt en utilisation nomade. Vanilla pèche vraiment trop sur la qualité sonore, surtout dans certains types de musique et la gestion de la bibliothèque est énervante. Musicolet reste un bon choix pour qui ne sera pas trop soucieux de la qualité du son, par exemple sur un téléphone bas de gamme en nomade. Il faut noter aussi qu'en écoutant du streaming bas de gamme (bref, pas Qobuz ou Tidal) ou des MP3 hasardeux, la plupart suffiront à votre bonheur.

![image](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2018/pulsar.jpg)

*Pulsar en action*
