---
layout: post
title: Tuto - "Voir" les répertoires de son NAS au démarrage sous Debian
category: tuto
tags: debian, linux, logiciel libre, nas, synology, tutoriel, 
---

**Il y a d'autres solutions que celle là, mais celle-ci fonctionne. Je ne suis pas passé par la solution Samba car il s'agit d'un format Microsoft. Donc j'ai utilisé la fonctionnalité nfs de mon NAS synology.**

L'objectif est d'avoir **les répertoires usuels du NAS accessible directement sur le bureau** ou dans son gestionnaire de fichier. C'est une demande souvent faite par des utilisateurs néophytes qui ne comprennent pas le principe du "montage" avec leurs habitudes de Windows. Evidemment, ils ne seront pas root/admin mais seulement utilisateurs.

Au préalable, il est nécessaire d'avoir défini **une adresse IP fixe** sur le réseau domestique pour le NAS. Chaque box a son interface mais il vous faudra trouver l'adresse MAC inscrite sur le NAS ou dans son interface. Dans mon exemple, le XX sera à changer par le numéro choisi pour votre NAS. Ensuite, il faut aller dans l'interface du NAS, dans mon cas c'est un Synology et ça ressemble à ça : <a href="https://www.synology.com/fr-fr/knowledgebase/DSM/tutorial/File_Sharing/How_to_access_files_on_Synology_NAS_within_the_local_network_NFS">TutoSyno.</a>

Ouvrez ensuite **un terminal** et tapez
>sudo mousepad /etc/fstab

rajoutez les lignes

>192.168.0.xx:/volume1/music /mnt/music/       nfs     users,atime,auto,rw,dev,exec,suid 0 0
>192.168.0.xx:/volume1/photo /mnt/photo/       nfs     users,atime,auto,rw,dev,exec,suid 0 0
>192.168.0.xx:/volume1/video /mnt/video/       nfs     users,atime,auto,rw,dev,exec,suid 0 0

notez aussi que mousepad est un exemple puisqu'un autre éditeur de texte fonctionne aussi pour modifier fstab.

**Attention à bien respecter la syntaxe, notamment pour le "volume1" qui doit correspondre au nom du disque dans le NAS.**

Il ne vous reste plus qu'à inclure des raccourcis pour ces répertoires, si vous le souhaitez.
