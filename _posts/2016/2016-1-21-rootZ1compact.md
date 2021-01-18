---
layout: post
title: Tuto - Rooter et sécuriser son XPeria Z1 Compact (ou son androphone)
category: tuto
tags: android, D5503, firewall, mobile, root, sécurité, sony xperia, turoriel, Tutoriels, Z1 Compact
---
**Après quelques déboires de mises à jour sur mon Sony Xperia Z1 Compact, qui perdait de 50% d'autonomie avant d'avoir une batterie chauffant anormalement,  je l'ai repassé en Rom Android 4.4.4 build 157, avec le tutoriel de <a href="http://www.phonandroid.com/forum/installer-un-firmware-officiel-sur-sony-xperia-z1-compact-d5503-t84638.html#p1263743">Phonandroid</a>. Le problème d'autonomie n'a été soldé que par un changement de batterie. Restait maintenant à le rooter et installer un firewall (qui lui est valable pour n'importe quel téléphone Android rooté).**

### Root

Avec cette version d'Android, pas de souci à avoir, puisqu'un tutoriel existe. Il est évidemment conseillé de tout sauvegarder au préalable. Première étape : Installer <a href="http://www.flashtool.net/downloads.php">Flashtool</a> sur un PC Windows. Puis télécharger les différents kernel nécessaires qui sont indiqués sur la page. Tout est expliqué dans ce tutoriel encore sur <a href="http://www.phonandroid.com/forum/rooter-le-xperia-z1-compact-en-4-4-4-firmware-157-bl-verrouille-compatible-t105818.html">Phonandroid</a>. :

* Eteindre le téléphone
* Utiliser flashtool pour mettre le Kernel 108
* Rallumer le téléphone en appuyant sur volume bas avant
* Utiliser RootkitXperia....

Mais ce tutoriel n'est pas totalement opérationnel car la version d'ADB n'est pas à jour. J'ai donc utilisé <a href="http://adbshell.com/downloads">celle-ci</a>. Ensuite on peut poursuivre l'utilisation de RootkitXperia qui est <a href="http://www.phonandroid.com/forum/rootkitxperia-methode-de-root-facile-des-xperia-2013-et-2014-bl-verrouille-t96821.html">décrite ici</a>.

* Le téléphone reboote et on le rééteint
* On réutilise flashtool pour mettre le kernel 157
* On rallume comme indiqué
* Et c'est fait.

### Le Firewall

Le terme firewall n'est pas forcément approprié, par rapport à tout ce qu'il y a à gérer sur Android. En effet, en plus de la gestion des ports réseau, il y a aussi à gérer les permission des applications sur d'autres applications du téléphone., comme les SMS, la liste de contact, etc... Du temps de mon X10 mini et sur le ZTE Blade en Android 2.3, j'avais pris l'habitude d'utiliser la rolls du firewall : **LBE Privacy Guard**, un programme fabuleux pour tout contrôler programme par programme mais qui ne fonctionne que sur les versions d'android inférieures à 3.0..... Depuis le développeur chinois Lamian a sorti un **LBE Security Master**, disponible en chinois sur le playstore. Mais Heureusement, XDA a développé une version anglaise qui a donné ensuite une version française, disponible.... devinez où ? Oui, encore sur <a href="http://www.phonandroid.com/forum/app-lbe-security-master-root-requis-application-multifonctions-t68378.html">Phonandroid</a>. Mais attention, la bonne version à télécharger se trouve dans la dernière page du sujet.

<img src="http://www.lbesec.com/static/images/lbe3/security_fun/fun3/04.png" alt="" width="226" height="402" />

Le programme est maintenant encore plus complet (et complexe?) avec un antivirus, une gestion des applications démarrant automatiquement, mais toujours la possibilité de gérer toutes les permissions des applications une par une. Je vous conseille d'en lire patiemment le tutoriel de Phonandroid, qui permet de comprendre tout le package. Aucun firewall du playstore n'arrive à ce résultat en terme de convivialité, pas même <a href="http://forum.xda-developers.com/xposed/modules/xprivacy-ultimate-android-privacy-app-t2320783">XPrivacy</a> qui pourra pourtant satisfaire quelques uns. Ajoutons à cela la suppression des pubs et adwares (enfin presque...) et surtout le fait d'empêcher le démarrage automatique des applications et c'est le rêve. Pas étonnant que le top des constructeurs chinois (Xiaomi, Meizu) utilisent le produit. Bonus, il gère même le spam SMS.

Après tout ça, Google, Yahoo et les autres vont vous maudir... Effet de bord de l'utilisation de LBE, un bug des roms 4.x des Xperia a disparu : Les applis qui démarrent toutes seules à la fermeture d'une autre appli. A ce sujet, il est conseillé de mettre la messagerie free en liste blanche
