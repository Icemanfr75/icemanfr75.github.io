---
layout: post
title: Tuto - Switcher sous Linux Etape 4 - L'installation
category: tuto
tags: distribution, installation, linux, logiciel libre, tutoriel, tuto
---
**Après avoir découvert la distribution linux qu'il vous faut à travers un LiveCD, vous allez enfin pouvoir installer votre système sur le disque dur du PC. Cet article n'a pas vocation a être un guide d'installation mais à montrer les quelques difficultés que vous pourrez rencontrer.**

Vous êtes donc en train de tester le Live CD de votre choix. Selon les distributions, la procédure est différente. Certaines obligent à redémarrer du CD/DVD pour choisir l'installation avec même des options de personnalisation. D'autres vont permettre cela directement à partir du live CD.

Mais il reste un problème de taille pour le néophyte : faire de la place sur le disque dur. Car installer un autre système, c'est le faire sur ce que l'on appelle une partition du disque dur. La plupart du temps, un disque dur est constitué d'une seule partition égale à sa capacité maximale. Cette partition n'est pas utilisée au maximum. Il faut donc récupérer cet espace libre afin de l'utiliser pour une partition linux qui n'est pas dans le même format que windows (NTFS ou FAT).

Dans les distributions récentes, un outil permet de redimensionner tout cela sans perte de données lors de l'installation. C'est plus ou moins pratique d'ailleurs et les termes ne sont pas des plus clairs pour les distributions les plus professionnels. Sachez également qu'il est conseillé de créer une partition de Swap égale au minimum à la taille de la mémoire vive du PC et souvent le double. Sous Windows, cet espace est alloué par le système de manière invisible mais existe aussi.

Maintenant que vous avez compris l'essentiel, lancez l'installation. Un mot de passe va vous être demandé pour le compte Root puis il vous sera demandé de créer un compte utilisateur avec un mot de passe différent. C'est avec ce compte que vous utiliserez votre Linux, le root ne servant qu'à faire des installations éventuelles et quelques configurations. L'installation des distributions modernes n'est pas beaucoup plus compliquée que celle d'un Windows ou d'un OSX. Les interfaces sont graphiques et comme vous avez testé le liveCD, votre matériel devrait être reconnu de la même manière.

Mais vous avez une question à régler : comme vous gardez encore votre ancien système windows, il va yavoir un choix au démarrage entre le linux et windows. C'est ce qu'on appelle le boot loader. Lors de l'installation, il vous est proposé d'en installer un et de choisir le système qui se chargera par défaut. Libre à vous de choisir votre préférence, sachant que l'édition d'un fichier suffira ensuite à changer cette option. Maintenant il ne vous reste plus qu'à redémarrer et de choisir Linux au démarrage du PC.

Après le premier démarrage, vérifiez tout de même que tout fonctionne, que les langues sont bien configurées et que vous voyez votre partition windows. Elle n'est pas forcément systématiquement montée mais reste visible dans le gestionnaire de fichier. Maintenant, à vous les joies de la découverte d'un nouveau système
