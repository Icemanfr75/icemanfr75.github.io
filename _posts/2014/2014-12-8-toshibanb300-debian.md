---
layout: post
title: Tuto -  Faire fonctionner un Netbook Toshiba NB300 sous Debian Wheezy
category: tuto
tags: debian, linux, toshiba nb 300, tutoriel,
---
**Les possesseurs de cette Machine voudraient souvent bien se passer du Windows 7 Starter d'origine mais ne savent pas quel système d'exploitation utiliser. Entre les ressources limitées (CPU, mémoire) et le choix pléthorique de l'offre du monde Linux, voici mon choix.**

Le NB300 a fonctionné sous deux versions de Debian Wheezy : la XFCE et la LXDE. Il s'agit de deux choix d'environnement graphique légers, la LXDE utilisant 90 Mo de RAM à vide tandis que la XFCE en utilise 130. Au niveau du package logiciel, la XFCE est préférable pour un point : Elle intègre le power manager de XFCE, impératif pour gérer la fermeture du capot du netbook. Ce Power Manager est installable sur LXDE mais cela vous fera faire des manipulations supplémentaires. Je suis passé par le live CD de la Wheezy en XFCE (1Go), installé sur une clé USB avec Universal USB Installer. Il vous suffit juste de sélectionner le type d'OS, de lui dire où se trouve l'ISO sur votre disque dur, puis de faire l'installation sur le lecteur correspondant à votre clé USB (4 à 8Go pour être à l'aise). Une fois terminé, redémarrer le PC et appuyez sur F12 pour accéder au menu de boot. Sélectionner la clé USB et vous voilà dans un choix cornélien :

* Tester le système en Live avec cette clé. Cela peut être bien pour commencer et se faire un peu la main
* Faire une installation en mode normal (Install)
* Faire une installation en mode graphique (Graphical Install)

Si vous avez à repartitionner le Netbook, le mode graphique est préférable. Mais Peut être est-il préférable de faire le boulot sur Windows avec votre outil de partitionnement préféré. Les différentes possibilités d'installation sont proposées ensuite. Si vous n'êtes pas sur, passez par le mode débutant avec une seule partition pour tout. Cela choquera les puristes mais au moins, tout fonctionne. Il peut arriver que l'installateur ne détecte pas correctement le wifi. Dans ce cas, faites un retour en arrière et recommencez jusqu'à ce que tout soit bien détecté. Sinon passez par un cable ethernet . Pour le bootloader Grub, c'est à dire ce qui va s'afficher au démarrage, n'oubliez pas de bien indiquer le disque dur principal dev/sda (ou éventuellement une carte SD /dev/sdc... dans ce cas, n'installez pas grub dans le MBR ). Normalement, après une bonne demi heure, l'installation se termine et vous demande d'enlever votre clé USB. A ce moment, c'est l'angoisse....Grub s'affiche, vous sélectionnez la première option, et la fenêtre de connexion s'affiche en vous demandant de vous identifier. Tout n'est pas terminé pour autant puisque la moindre mise en veille vous causera un plantage. Il y a moyen d'y remédier. (valable aussi pour Ubuntu &gt;10.4 et dérivés de Debian)

* Connectez vous sous le nom Root avec le mot de passe défini lors de l'installation. Ouvrez un terminal.
* Tapez d’abord : sudo mousepad /etc/default/grub ce qui va ouvrir l’éditeur de texte mousepad. Pour un bureau gnome, ce sera Gedit, etc...
* Changez la ligne suivante : GRUB_CMDLINE_LINUX_DEFAULT=”quiet splash nolapic_timer clocksource=jiffies”
* Sauvez la modification
* Tapez dans le terminal : sudo update-grub
* Tapez dans le terminal : sudo reboot now
* Le PC va rebooter.

Maintenant, il vous faut aller sur le Power Manager pour définir comme va s'éteindre le PC selon qu'il sera branché ou pas. L'interface graphique est très claire. Je vous déconseille par contre l'hibernation ou veille prolongée qui semble ne pas bien fonctionner. Après ça vous avez un Netbook qui démarre vite, a tout le pack logiciel nécessaire à une utilisation standard. Et surtout il n'est plus autant vulnérable aux chevaux de troie et virus.
