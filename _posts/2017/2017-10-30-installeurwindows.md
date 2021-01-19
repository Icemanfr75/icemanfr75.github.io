---
layout: post
title: Tuto - Créer un installateur Windows pour autre chose qu'une application
category: tuto
tags: informatique, installeur, tutoriel, Tutoriels, windows
---
**Vous allez me dire, quelle drôle d'idée... Mais imaginez que vous êtes dans une entreprise sans le moindre accès à un serveur pour faire un "portail web", et bien la seule solution est d'installer en local des fichiers sur chaque poste. Si vous n'êtes pas administrateur du parc, oubliez alors l'automatisation et pensez au bon vieil installateur Windows. Sauf que cette fois, vous n'installez pas un logiciel mais quelques fichiers HTML et images.**

Mon but était de **proposer une page d'entrée** pour les utilisateurs de mon service donnant accès autant aux outils nécessaires de l'entreprise que quelques fichiers hébergés dans le système d'archivage interne, et des liens vers l'extérieur. Le rythme de mise à jour est faible. On a donc des fichiers excel, des annuaires, des liens vers les ressources humaines, les systèmes de commande de pièce, etc...Le tout est réparti en rubriques avec un "look" pas trop décallé par rapport aux standards. J'aurais pu faire une simple page de liens HTML pure et dure mais j'ai fait ça avec des sous-pages en frame, à l'ancienne quoi, sans passer par des feuilles de style. Pourquoi? Tout simplement parce que c'est plus simple à éditer par un néophyte avec des outils gratuits avec une structure claire, une aide intégrée expliquant le rôle de chaque fichier html.

* Pour éditer les pages, je passe par <a href="http://www.kompozer.net/">Komposer</a> ou <a href="http://www.bluegriffon.org/">Blue Griffon</a> qui sont des outils libres.
* Pour faire l'installeur, je passe par <a href="http://www.jrsoftware.org/isinfo.php">Inno Setup</a>, un autre outil libre.

Je vais donc détailler le principe pour l'installeur qui est plutôt prévu pour des logiciels à la base.

1°) faire un répertoire pour tous les fichiers à installer. Je conseille d'avoir un répertoire \img pour les images par exemple, et un répertoire \pages pour ce qui  sera à éditer, le reste étant par exemple dans \structure ou dans \menu.

2°) quand vous lancer Inno Setup pour la première fois, vous avez un Script Wizard qui vous aide pour l'essentiel... il est en anglais mais permet de faire des installeurs dans beaucoup de langues. Mais comme on des warriors, on va en faire un vide  (create a new empty script).

![image](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2017/inno1.jpg)

On se retrouve alors avec une grande fenêtre bien vide. Je vous propose de copier dedans les lignes suivantes :
>[Setup]
>; NOTE: The value of AppId uniquely identifies this application.
>; Do not use the same AppId value in installers for other applications.
>; (To generate a new GUID, click Tools | Generate GUID inside the IDE.)
>AppId={{xxxxxxxxxxxxxxxxxxxxxxxxxxx}}
>AppName=Portail
>AppVersion=1.0.0
>AppVerName=Portail 1.0.0
>AppPublisher=Mon Nom
>AppPublisherURL=xxxxxx
>AppSupportURL=xxxxxx
>AppUpdatesURL=xxxxx
>DefaultDirName=C:\User\
>DefaultGroupName=Portail
>OutputDir=C:\User\
>OutputBaseFilename=portail
>Compression=lzma
>SolidCompression=yes
>SetupIconFile=C:\User\Moi\site\img\logo.ico
>
>[Languages]
>Name: "french"; MessagesFile: "compiler:Languages\French.isl"
>
>[Files]
>Source: "C:\User\Moi\site\*"; DestDir: "{app}"; Flags: ignoreversion recursesubdirs createallsubdirs
>; NOTE: Don't use "Flags: ignoreversion" on any shared system files
>
>[Icons]
>Name: "{group}\Lancer le Portail"; IconFilename: "{app}\img\logo.ico"; Filename: "{app}\index.html"
>Name: "{group}\Désinstaller le portail"; Filename: "{uninstallexe}"
>Name: "{userfavorites}\Portail SOMI"; IconFilename: "{app}\img\logo.ico"; Filename: "{app}\index.html"
>
>[Run]
>Filename: "{app}\index.html"; Description: "lancer le portail"; Flags: postinstall shellexec

Sauvegardez le script où vous voulez avec un nom qui vous parle, genre portail.iss

### Maintenant détaillons un peu :

Le [Setup] concerne l'installeur proprement dit.

* L'appID permet d'identifier l'application par un numéro unique qui peut se générer en allant dans le menu TOOLS/Générate GUID
* DefaultDirName est le répertoire proposé par défaut par l'installeur
* DefaultGroupName est le nom du groupe qui sera créé dans le menu démarrer de windows
* OutputDir est le répertoire où sera créé l'installeur (le fichier .EXE)
* OutputBaseFilename est le nom du fichier
* SetupIconFile est une possibilité de rajouter une icône... ici je prends dans mon répertoire image

La Rubrique [Files] concerne les fichiers qui seront installés. Je conseille de les mettre dans le même répertoire, comme par exemple ici "Site". Il seront installer dans le répertoire {app} qui correspond à au répertoire d'installation qu'a choisi l'utilisateur.

La Rubrique [Icons] correspond aux raccourcis que le programme va installer:

* Name définit le nom qui sera affiché pour ce raccourci et sa localisation. Par exemple {group} prend l'emplacement du groupe du menu démarrer. {userfavorites} correspond aux favoris internet du navigateur par défaut.
* IconFilename permet de définir l'icône du raccourci. Ici c'est mon logo de mon répertoire image \img
* Filename permet de définir la cible. Ici j'ai donc l'index.html qui permet de lancer le portail. J'ai aussi le désinstalleur.

La Rubrique [Run] permet de définir ce qui sera lancé en fin d'installation. Par exemple ici, je lance mon fichier index.html et l'utilisateur pourra décocher tout ça.

Vous allez me dire après... **Mais si on n'est pas sous windows?**

Je n'ai pas de Mac dans mon parc mais si j'avais un PC Linux, je me contenterai d'une simple archive car l'utilisateur est souvent un peu plus apte à gérer ça que ceux que j'ai sous Windows. A savoir que 7Zip permet aussi de faire une archive autoextractible (SFX) pour Windows, pour ceux que ça rebute.

### Et après?

La mise à jour peut se faire par un simple lien pointant sur l'Executable ou l'envoi du .EXE, le programme reconnaissant l'emplacement défini après installation et écrasant par défaut les fichiers. Mais vous pouvez recommander la désinstallation avant si des raccourcis ont changé de nom, par exemple, ou si vous avez supprimé des fichiers.

En tout cas, ça fait quelques années que je fonctionne avec ça et les utilisateurs sont plutôt contents d'avoir l'essentiel à portée de main. On fait juste des révisions périodiques des besoins avec eux.
