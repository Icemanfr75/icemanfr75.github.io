---
layout: post
title: GNU Linux - Distributions, Netbook et Optimisation
category: geek, tuto
tags: debian, distribution, fedora, Geekeries, linux, linux mint, logiciel libre, netbook, toshiba nb 300, Tutoriels, ubuntu
---
**Suite à mon coup de gueule tuto sur XFCE et Thunar, je suis parti à nouveau sur la piste d'un couple OS/Gestionnaire de fichier qui convienne à la fois à un débutant, à une machine ancienne et surtout à un netbook (il y en a des tonnes en occasion), voire un mini ordinateur. Un bilan de l'utilisation mémoire par environnement, et quelques surprises...**

**Préambule**
Je sais qu'à l'heure des tablettes et hybrides, on se fout de tout ça mais le mien, malgré ses particularités en <span style="text-decoration:underline;"><a href="https://fr.wikipedia.org/wiki/Advanced_Configuration_and_Power_Interface">ACPI</a>, fonctionne bien avec ses 2 GO de Ram (attention, la plupart en ont 1Go) et son disque d'origine, et ses 6 ans d'age. La difficulté est d'avoir donc la gestion d'un écran en 1024x600 à l'installation, une consommation mémoire que je voudrais la plus faible, tout autant qu'une consommation processeur pas trop gourmande en "Idle" (bref, en ne faisant rien d'autre qu'afficher l'OS). Tout cela sans faire moins qu'un Windows XP/7 d'origine sur ce type de machine, à savoir bureautique, internet, petite retouche ou classement photo, connection à un <span style="text-decoration:underline;"><a href="https://cheziceman.wordpress.com/2016/04/26/tuto-voir-les-repertoires-de-son-nas-au-demarrage-sous-debian/">NAS au démarrage</a>. Donc, plutôt que de faire une vidéo en virtualbox qui mettrait à genou mon système, j'ai préféré la bonne vieille méthode de la clé USB en live et regardé les points forts et points faibles de ce qu'il y avait sur le marché. J'ai pris des copies d'écrans de chacun sur la conso mémoire et processeur avec les outils de monitoring fournis. Je compare à ma vieille debian 7 XFCE pour référence : **121 Mo de Mémoire consommée !**
Pour ceux qui s'étonnent que je fasse ce test avec une optique d'économie et de réutilisation de machines, il faut se souvenir que **GNU Linux n'a jamais été aussi bon que dans la réutilisation de vieux matériels **(ou même de mini ordinateurs comme les Raspberry Pi)**.** Les pilotes sont souvent existants et éprouvés et le marché est abandonné par les systèmes commerciaux. Mais paradoxalement, les leaders du "monde libre" que sont Mint, Ubuntu, Fedora, continuent la course à l'armement au lieux de faire des systèmes plus Lean, pour reprendre un terme à la mode il y a quelques années. L'essentiel est aussi, pour moi, d'avoir un système très simple d'accès, fiable dans le temps, pour pouvoir fournir une machine clé en main à un débutant. <span style="text-decoration:underline;"><a href="https://debian-facile.org/">Debian Facile</a> s'y attache aussi à sa manière mais n'est pas là pour faire des reviews d'environnement graphiques. Ma philosophie n'est pas non plus d'aller chercher un sombre fork mais d'utiliser un OS d'une branche principale ou d'un seul niveau de fork (Debian, Ubuntu, Centos, Fedora, Archlinux....si ça avait pu être possible, même avec les excellents tutos de Frederic Bezies). Je fais une incartade avec Linux Mint. En théorie, on dirait aussi pas d'OS 64 bits non plus, vus les processeurs visés. Pas besoin de Flash intégré, vu le peu d'avenir de cette technologie.
Les heureux élus sont donc :

 	* Debian 8 Mate i386 et AMD64
 	* Debian 8 Cinnamon
 	* Debian 8 Gnome
 	* Xubuntu 16.04
 	* Ubuntu-Mate 16.04
 	* Fedora 24 (Gnome et KDE)
 	* Centos 6.8 (Gnome2)
 	* Linux Mint 18 Cinnamon

**Consommation mémoire**
Elle devrait idéalement être inférieure à 400 Mo, sachant que ma Debian 7 XFCE était à 121 et que mon Windows 7 SE sur la même machine était à 806Mo avec le même genre de tache de fond au démarrage. Je n'ai pas mesuré le temps de démarrage car je n'ai pas pu utiliser toujours le même périphérique mais Windows reste le plus lent avec la Fedora 24 évidemment qui représente l'OS moderne. Attention, ces chiffres seront différents sur une machine dotée d'1Go de mémoire. Le résultat est le suivant :

<table border="1" width="60%">
<tbody>
<tr>
<td>Debian 7 XFCE</td>
<td>121 Mo</td>
</tr>
<tr>
<td>Debian 8 Mate</td>
<td>182 Mo</td>
</tr>
<tr>
<td>Centos 6.8 Gnome2</td>
<td>220 Mo</td>
</tr>
<tr>
<td>Debian 8 Mate 64bits</td>
<td>250 Mo</td>
</tr>
<tr>
<td>Xubuntu 16.04 LTS</td>
<td>273 Mo</td>
</tr>
<tr>
<td>Debian 8 Cinnamon</td>
<td>300 Mo</td>
</tr>
<tr>
<td>Linux Mint 18 Cinnamon</td>
<td>354 Mo</td>
</tr>
<tr>
<td>Debian 8 Gnome</td>
<td>371 Mo</td>
</tr>
<tr>
<td>Ubuntu Mate 16.04 LTS</td>
<td>587 Mo</td>
</tr>
<tr>
<td>Fedora 24 Gnome</td>
<td>685 Mo</td>
</tr>
<tr>
<td>Fedora 24 KDE</td>
<td>710 Mo</td>
</tr>
<tr>
<td>Windows 7 SE</td>
<td>806 Mo</td>
</tr>
</tbody>
</table>
Le constat est sans surprise (XFCE&lt;Mate&lt;Cinnamon&lt;Gnome&lt;KDE) et on peut être étonné du score de la Fedora en Gnome. Par contre, entre les deux versions de Mate, il y a 400Mo d'écart ce qui ne peut s'expliquer par le simple changement de kernel. On peut voir à l'inverse assez peu de différence entre la Debian 8 Cinnamon et la Linux Mint 18. Il faut dire qu'il y a beaucoup de superflu dans une Ubuntu, que Mint a trié. Une installation réelle devrait confirmer ou pas cet état de fait. Une chose est sûre : Le déchargement mémoire reste extrèmement rapide sur les Debian alors que les autres ont du mal à revenir au niveau d'origine en IDLE. Et passer en version 64 bits induit une charge mémoire plus importante (70Mo sur la Debian 8 Mate)


<img class="wp-image-7425 size-full" src="https://cheziceman.files.wordpress.com/2016/08/debian648mate.png" alt="debian648mate" width="605" height="457" />
Précision importante : Les chiffres sont issus des system monitors des différents systèmes. Ils comptent la mémoire cache dans la mémoire libre, ce qui change le constat si on utilise la ligne de commande TOP. Toutefois, c'est comparable à ce qu'affiche Windows.

**Utilisation du processeur****
J'ai été confronté à une question technique sur ce processeur Atom N450, monocoeur mais Multithread. Sur Fedora et Ubuntu-Mate (Kernel 4.x), j'ai deux CPU qui apparaissent, un peu comme dans Windows7 ce qui n'est pas totalement vrai. Dans les Debian 8 (Kernel 3.x), je n'en ai qu'un. Il semble que je ne sois pas le seul dans ce cas, mais ça dépend énormément des machines. Certaines avec des processeurs Atom comparables affichent bien deux CPU en kernel 3.X. Mais d'un autre coté, le kernel linux a officiellement été optimisé pour les processeurs Intel Atom depuis le kernel 4.1. En étudiant le cas de ce N450 on s'apperçoit alors qu'il est Intel64, donc il faut utiliser les versions AMD64 des Debian et non les versions 386 ou au moins intégrer le package 686 PAE. Et dans ce cas, on a les deux coeurs qui s'affichent et des performances bien plus surprenantes. Autre étrangeté, Centos et son kernel 2.6 affiche aussi 2 CPU, mais identifiés CPU0 et CPU1.

<table border="1" width="60%">
<tbody>
<tr>
<td>Debian 7 XFCE</td>
<td>2%</td>
</tr>
<tr>
<td>Debian 8 Mate AMD64</td>
<td>4%</td>
</tr>
<tr>
<td>Centos 6.8</td>
<td>5%</td>
</tr>
<tr>
<td>Xubuntu 16.04 LTS / Debian 8 Mate i386</td>
<td>14%</td>
</tr>
<tr>
<td>Linux Mint 18 Mate</td>
<td>14%</td>
</tr>
<tr>
<td>Ubuntu Mate 16.04 LTS</td>
<td>15%</td>
</tr>
<tr>
<td>Linux Mint 18 Cinnamon</td>
<td>18%</td>
</tr>
<tr>
<td>Windows 7SE</td>
<td>23%</td>
</tr>
<tr>
<td>Fedora 24 KDE</td>
<td>24%</td>
</tr>
<tr>
<td>Fedora 24 Gnome</td>
<td>25%</td>
</tr>
<tr>
<td>Debian 8 Cinnamon/Gnome i386
</td>
<td>43%</td>
</tr>
</tbody>
</table>
Le Swap a été utilisé légèrement sur Fedora et Ubuntu-mate alors qu'il ne sert à rien sur Debian, qui consomme, d'un autre coté, moins de ressources mémoires. En faisant tourner un peu plus le proc (compression, décodage vidéo et internet), j'ai eu moins de ralentissement sur les Kernel 4.x. Sur la Ubuntu Mate, la conso mémoire grimpe très vite dans des proportions astronomiques (Jusqu'à 1.6Go avec Gimp en UbuntuMate pendant que je restais à 250Mo sur ma Debian XFCE sur la même action et même sur la Mint Cinnamon).


<img class="wp-image-7394 size-large" src="https://cheziceman.files.wordpress.com/2016/08/centos2.png?w=730" alt="centos2" width="730" height="428" />

**La recherche de fichiers****

Je rappelle que l'objectif est de rechercher des fichiers sur un disque et de pouvoir manipuler le résultat de cette recherche comme n'importe quel fichier (suppression, copier, coller, déplacer, taille de l'ensemble...). Oublions tout de suite XFCE qui même dans sa version xubuntu incluant catfish reste préhistorique sur ce domaine (pas de traitement de plusieurs fichiers en même temps). Pour les autres, rien à dire, ça fonctionne. Je suis peut être moins fan de l'interface KDE ou Gnome2, malgré les larges possibilités offertes. Il m'a semblé tout de même que Gnome3 et Cinnamon étaient plus rapide et pertinent, malgré la charge du système.

**Bilan par Système**

<img class="size-large wp-image-7393" src="https://cheziceman.files.wordpress.com/2016/08/centos.png?w=730" alt="Centos 6.8 et son Gnome2 en action" width="730" height="428" />

Je commence par **CentOS** que j'ai éliminé de mes choix pour un point : Pas de support du NTFS en natif dans le liveDVD. Ce n'est pas rédhibitoire si on a un environnement homogène et ça peut se corriger. Donc je comprends le choix dans la philosophie CentOS que je testais plus par curiosité. Pour le reste, on est sur du classique, du robuste à défaut de glamour, vu qu'on reste en Gnome2. Curieusement, malgré la faible charge processeur et mémoire, le système de liveDVD n'utilisait pas de swap et souffrait de ralentissements. Il pourrait s'agir du prix à payer pour utiliser le vieux kernel 2.6, peu adapté aux processeurs Atom.

<img class="wp-image-7378 size-full" src="https://cheziceman.files.wordpress.com/2016/08/windows7se.png" alt="windows7SE" width="504" height="456" />

J'élimine aussi **Debian 8 XFCE et Xubuntu** pour le <span style="text-decoration:underline;">problème de recherche de fichiers. Même Xubuntu qui intègre catfish ne permet pas grand chose sur le résultat d'une recherche. On est clairement dans un système qui n'a pas su évoluer avec son temps et n'est pas non plus assez poweruser aujourd'hui (pourquoi ne pas aller voir du coté d'Archlinux... ). Mais pour qui s'oriente sur une activité avec peu de manipulation de fichiers, ça peut être encore jouable.

<img class="wp-image-7379 size-large" src="https://cheziceman.files.wordpress.com/2016/08/xubuntu16lts.png?w=730" alt="xubuntu16LTS" width="730" height="428" />

Passons maintenant au challenger tout désigné : **Mate** et sa refonte du (bon) vieux Gnome2. Si j'ai testé en Debian et Ubuntu, c'est pour voir la différence, sachant que le premier est donc en kernel 3.x et le second en kernel 4.x. 400Mo (ou 300 en 64 bits) de mémoire de différence et des packages surperflus sur **Ubuntu.** Cela dit, le portage de Mate est remarquable sur cette version 16.04LTS avec un bon support du français à l'installation, des outils vraiment pratiques pour les débutants. Coté **Debian**, on reste sur quelque chose qui ne bouleverse pas les habitudes, de fiable, mais qui ne bénéficie pas des dernières versions logicielles, notamment Firefox qui reste en Iceweasel 38.8 (ça peut se corriger en incluant un dépot Mozilla...). Si on veut plus, il faut prendre une version instable du système.

**Cinnamon** peut être une alternative intéressante. C'est plus une histoire de goût, vu le peu d'écart avec Mate. Mais la rapidité de la **Linux Mint 18** est bluffante par rapport à un Ubuntu. Reste un bémol : Il faut installer le support du MP3 qui n'est pas présent sur le liveDVD, ce qui est incompréhensible dans une distribution orientée "out of the box", même si cette liberté ne me déplait pas. Cela peut se faire durant l'installation, par contre. La charge processeur est excellement gérée et il n'y a aucune anomalie mémoire dans l'utilisation de Gimp. Mais les temps de réponse pour des actions simples sont parfois trop longs, ainsi que le temps de déchargement mémoire.

<img class="wp-image-7392 size-full" src="https://cheziceman.files.wordpress.com/2016/08/mint18cinna.png" alt="mint18cinna" width="693" height="521" />

**Gnome** dans sa version 3 est une approche intéressante pour celui qui veut le dernier cri, de la performance en recherche, une interface novratice. Mais ça se paye en ressource. Que cela soit dans une Debian ou une Fedora, ça reste équivalent en terme d'interface. Je ne suis pas fan du coté rolling release (semi) de la Fedora (j'ai eu quelques couacs par le passé). Donc c'est un choix philosophique entre une distrib en retard et plus figée et une autre qui fait la course en tête. On peut aussi disserter sur les outils propres aux 2 branches de GNULinux et leur support de matériel. Comme je recherche la stabilité avant tout, vous aurez compris mon choix.

**KDE** fut autrefois (quand j'étais jeuuunnne....) ma tasse de thé mais ne l'est plus. A la fois trop classique et gourmand, je n'en vois pas l'intérêt dans mon optique. Après, je comprends que l'environnement perdure, mais c'est un autre sujet.

**CONCLUSION** : Mon choix se porte sur la Debian Mate AMD64. Je vais poursuivre mon choix en faisant une vraie installation jusqu'au bout avec tout ce que je juge strictement nécessaire.  En ce qui concerne les Raspberry Pi, il faut se souvenir que la Raspbian est basée sur une Debian 8 mais avec une optimisation pour les processeurs ARM de cette plateforme, qui semblerait aussi intégrée dans la Ubuntu Mate. Si je perds un peu par rapport à la Debian 7 que j'ai actuellement, cela reste tout à fait raisonnable, même pour une machine à 1Go de RAM. Reste à gérer les subtilités des chipsets, notamment la veille, voir le Wifi pour certains.

Pour le reste, j'ai apprécié particulièrement la Ubuntu-Mate 16.04 LTS et la Linux Mint 18 Cinnamon qui restent des bons choix sur des machines moyennes pour des utilisateurs débutants.
