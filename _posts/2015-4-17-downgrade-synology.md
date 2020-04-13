---
layout: post
title: Tuto - Downgrader un NAS Synology DS210J
category: tuto
tags: downgrade, dsm4, mise à jour, nas, synology, tutoriel
---
**Un petit #tutoriel pour les possesseurs de #NAS #synology : Comment enlever ce satané DSM5 pour revenir à un DSM4 sur un vieux DS210J**

Tout parait simple : On active Telnet et SSH dans le panneau de configuration de DSM... Mais il ne faut pas oublier de mettre aussi les droits d'utilisation sur le SSH dans le firewall/pare feu. On se connecte en SSH dessus avec l'adresse IP du NAS et là, le piège. Tout le monde dit qu'Admin et Root c'est pareil. Et bien non, pas chez moi. Donc on se connecte en root en utilisant le mot de passe ... d'admin. Ensuite, il faut avoir créé un fichier VERSION quelque part avec le contenu suivant :

>majorversion="4.3"
>minorversion="0"
>buildphase="3"
>buildnumber="3810"
>smallfixnumber="0"
>builddate="2013/11/21"

je vous conseille tout de même de taper more /etc.defaults/VERSION pour sauver l'ancienne version en la copiant quelque part. 3810, c'est l'avant dernier build de DSM4.... Il faut ensuite transférer ce fichier sur le NAS dans un répertoire genre public par exemple. Et là on tape alors la commande : cp /volume1/public/VERSION /etc.defaults/VERSIONOn va récupérer le fichier .PAT correspondant au build 3827 de DSM4.3<a href="http://dedl.synology.com/download/DSM/"> pour son NAS</a>. On se connecte sur le DSM avec adresse.IP:5000 et on va dans mise à jour. Le numéro doit alors etre 4.3 build 3810. On demande une mise à jour manuelle et on charge son fichier .PAT. Après une confirmation, il lance l'installation et revient à la version précédente qui bouffe moins de RAM pour les vieux NAS.

Attention, il peut être nécessaire de revoir les réglages du Firewall après installation du DSM4 ainsi que de désinstaller et réinstaller les paquets/packages, notamment le multimédia puis de réindexer les fichiers.

ps : pour les windowsiens qui connaissent pas telnet ou ssh, utilisez le logiciel putty.
