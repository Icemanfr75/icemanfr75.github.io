---
layout: post
title: Tuto - Comment récupérer ses enregistrements tv numérique ?
category: tuto
tags: adsl, encodage, enregistrement, tnt, tutoriel, Tutoriels, video
---
**Enregistrer sur une Freebox, c'est bien mais on veut parfois profiter de ses enregistrements sur d'autres terminaux comme par exemple des téléphones, tablettes, etc...Il existe maintenant une solution un peu plus simple pour le néophyte.**

*Attention, cette méthode ne fonctionne que pour les enregistrements auxquels on peut accéder via un PC en ftp. Les chaines comme TF1, M6, Canal+ ne rendent pas leurs enregistrements accessibles.*

### Récupérer l'enregistrement :

comme tout le monde n'a pas de logiciel FTP, le plus simple est tout simplement de taper l'adresse ftp://hd1.freebox.fr dans le navigateur (je ne connais pas les autres box mais cela doit être similaire). Un identifiant et un mot de passe sont demandés : l'identifiant est freebox et le mot de passe est celui que vous avez défini (ou pas) dans l'interface de paramétrage sur la télévision. Ensuite il suffit de trouver l'enregistrement dont le nom commence par la chaine de télé enregistrée.

### Ouverture et indexation du fichier :

Après un transfert assez long (il y a tout de même souvent plus de 2Go de données), on obtient un fichier en .ts. Il s'agit en réalité d'un MPEG. Le codage va être fait avec <a href="http://avidemux.berlios.de/">AVIDEMUX</a>, logiciel issu du monde linux et porté sur Windows. Il suffit d'ouvrir le fichier.ts dans AVIDEMUX pour qu'il propose d'abord une indexation du fichier. Faire OUI. Après  minutes, le fichier s'affiche dans la grande fenêtre.

### Calage de la vidéo

Comme l'enregistrement n'a pas commencé au début de l'émission et ne s'est pas terminé pile à la fin, il faut sélectionner la zone que l'on garde. Avec le curseur sous la vidéo, se positionner au début de l'émission et cliquer sur le bouton A. Puis aller à la fin de l'émission et cliquer sur le bouton B.

### Recodage du fichier :

Sur le coté gauche, il y a trois zones avec des boutons de sélection :
* Dans **video**, sélectionner d'abord le format XVID au lieu de copier. Cliquer sur configurer et sélectionner la méthode double passe avec filesize et taper 600 dans la taille du fichier pour une émission de moins de 2h. sélectionner l'aspect ratio comme à l'origine. Dans Filtres, sélectionner Resize et entrer décocher lock aspect ratio avant de rentrer le format 800x576 ou un multiple moins grand de 8 respectant ce format. Attention, cette valeur dépend aussi du format du programme selon qu'il est en 16/9 ou 4/3. Il faut vérifier la validité de cette valeur avec le bouton Apperçu.
* Dans **audio**, sélectionner mp3 Lame.
* Faire enregistrer une vidéo et taper le nom du fichier désiré en rajoutant .avi à la fin. Le codage se lance et il peut durer de 1 à 10h selon la taille de l'émission et la puissance de la machine.

### Vérification du positionnement du son

Il peut arriver que le son se décalle d'avec l'image. Parfois il suffit de rouvrir le fichier obtenu avec AVIDEMUX et de mettre tout en copier en mettant un décalage du son (zone de saisie à gauche sour la rubrique audio) à -1000ms (soit 1s). Il est possible de vérifier que ça marche en faisant directement la lecture du fichier dans AVIDEMUX ce qui aide beaucoup au réglage. Après avoir trouvé la bonne valeur, il faut réenregistrer la vidéo sous un autre nom et cela prend de 1 à 5 minutes.

Pour l'utilisation d'une vidéo xvid sur un ipod/iphone, il existe un programme spécialisé qui s'appelle <a href="http://www.clubic.com/telecharger-fiche18827-free-ipod-video-converter.html">Jodix Ipod video converter</a>. L'utilisation est simplifiée à l'extrème.


