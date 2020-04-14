---
layout: post
title: Tuto - Réinstaller un PC Windows du commerce
category: tuto
tags: pc, réinstallation, tutoriel, windows
---
**Après presque 4 ans d'utilisation, un des PC de la maison est fortement ralenti. Il est temps d'utiliser la fonction "Recovery" installée par le constructeur, autrement dit : La Réinstallation comme à l'origine. Mais encore faut-il prendre des précautions.**

Si la phase de recovery proprement dite est courte, ce sont les phases préparatoires et post-installation qui sont longues.

**Matériel nécessaire : **
* Une clé USB de 8 ou 16Go
* Un disque dur externe de 250 à 500Go (selon la taille des documents installés)
* Une bonne journée calme
* L'utilisateur habituel du PC
* Une feuille de papier
* Un stylo (si si, souvenez vous...)

**Phase 1 : Lister les logiciels installés**

Prenez la feuille de papier, le stylo et listez ce que vous voyez dans le menu "démarrer" de Windows. Allez ensuite dans le "Panneau de configuration", rubrique "Programmes et Fonctionnalités" et rajoutez les logiciels qui ne sont pas déjà listés. Allez voir/appelez l'utilisateur pour tout ce qui vous semble anormal. S'il ne connait pas, vous mettez un signe distinctif pour ne pas chercher à réinstaller plus tard ce logiciel. Pour tout ce qui est logiciel du commerce (Office de Microsoft par exemple), pensez à récupérer les DVD/CD d'origine à ce moment là. Sinon, il va falloir trouver des solutions en "libre" comme LibreOffice par exemple. Usez de diplomatie.

**Phase 2 : Passer un antimalware et un antivirus**

Même si tout va être effacé, il peut y avoir des virus et outres pouriciels dans les documents qui vont être sauvegardés. C'est donc le moment de sortir votre copain <a title="AntiMalware de Malwarebytes" href="http://r.duckduckgo.com/l/?kh=-1&amp;uddg=http%3A%2F%2Fwww.malwarebytes.org%2F">AntiMalware de Malwarebytes</a> , et d'utiliser l'antivirus qui devrait être installé...devrait mais parfois il va falloir faire dans le gratuit, faute de mieux, c'est à dire Windows Defender, Avira, etc... Pendant le scan, vous êtes tranquille pour faire autre chose et retrouver la vie réelle.

A l'issue, vous pouvez faire une **clé USB de Recovery** à l'aide de l'utilitaire du constructeur planqué dans le menu démarrer. Il est soit dans le répertoire ayant le même nom que le constructeur, soit dans les accessoires

avec un terme du genre Recovery media creator, Backup creator, Restauration ...sauf le "Restauration du Système" dans Accessoires/Outils Systemes qui est l'outil Windows.

Vérifiez aussi que vous avez tous les pilotes de matériel supplémentaire sur un support externe (CD, DVD, clé USB)...sinon cherchez les.

**Phase 3 : Sauvegarder les documents**

Attention, il y a peut-être plusieurs utilisateurs sur le PC. Pensez alors à sauvegarder chaque dossier situé dans C:/Users ou C:/Utilisateurs. Il faudra aussi récréer les utilisateurs dans la phase 7. Pour sauvegarder, il faut brancher le disque dur externe (correctement alimenté) sur un port USB, et copier tous les répertoires utilisateurs dedans. Vous pouvez au préalable créer un dossier sauvegarde avec la date, comme "Sauvegarde PC Toto 30-05-2015". Là vous risquez d'en avoir pour quelques heures, voir une nuit, ce qui vous obligera à placer le pc à un endroit où il n’empêche personne de dormir (vieux disque dur=disque dur bruyant).

**Phase 4 : Sauvegarde des Marque-pages/Bookmarks du navigateur**

Même si vous utilisez les fonctions de synchronisation de Firefox ou Chrome, il n'est pas inutile de sauvegarder aussi les bookmarks ou Marque-pages. Il faut aller dans l'interface de gestion du navigateur (Ctrl+maj+B par exemple sur Firefox) et utiliser la fonction "Sauvegarde".

**Phase 5 : Recovery**

Le point d'entrée normal est l'utilitaire de "recovery" installé par le constructeur qui fait appel à une partition cachée du disque dur. Dans un cas extrème, on peut avoir à utiliser la clé USB créée pour cela et à booter dessus (mode boot select au démarrage du PC). Dans tous les cas, on se retrouve dans une procédure automatisée après redémarrage qui ne demandera qu'un nom d'utilisateur, un nom de PC.... puis sélectionnera peut-être un réseau wifi par défaut.

**Phase 6 : Reinstallation du matériel**

Après un premier redémarrage, on se retrouve avec un PC tel qu'il était à l'achat, c'est à dire avec quelques produits promo, des outils inutiles, etc...Commencez par désinstaller l'antivirus en version d'essai, l'office en version limitée. C'est un minimum. Ensuite, installez les périphériques essentiels (Imprimante, Scanner...) et faites les mises à jour proposées par Windows Update.

**Phase 7 : Réinstallation des logiciels**

A l'aide de votre petite check list papier, il va falloir installer les logiciels. Commencez toujours par l'antivirus et/ou les logiciels de sécurité. Attention, pour tous les logiciels gratuits, il faut faire des installations personnalisées pour éviter d'avoir des pouriciels et malwares en même temps. Regardez toujours tout ce qui n'est pas le logiciel que vous installez, les cases cochées par défaut, etc... Après ça, faite dans l'ordre de votre liste en commençant par l'essentiel (bureautique, photo, musique... selon vos goûts) pour finir par le superflu. Vérifiez toujours le bon fonctionnement du logiciel en le lançant à l'issue de l'installation. Si vous avez téléchargé une nouvelle version, vous pouvez avoir des surprises. Réunissez tous ces téléchargements dans un répertoire de votre disque de sauvegarde : Ca peut servir pour la prochaine fois.

**Phase 8 : Recopie des documents**

Après toutes ces installations, il ne vous reste plus qu'à remettre tous les fichiers sauvegardés à l'emplacement d'origine. C'est beaucoup moins long que dans l'autre sens, en général. Et ça permet aussi de faire un premier tri. Attention, faites toujours un COPIER et pas un COUPER.

**Phase 9 : Passer un antimalware et un antivirus**

A l'issue de ces installations, une dernière vérification s'impose : Antivirus et Antimalware pour savoir si tout est normal. Là aussi on a des surprises, même sur les restaurations d'origine. Si vous avez installé un utilitaire d'image disque, faites une image de cette installation, cela gagnera encore plus de temps la prochaine fois dans une restauration. Sauvez cette image avec un nom explicite rappelant le type de PC, le nom de l'utilisateur, la date, etc...

Pour un PC sans Recovery, remplacez la phase de Recovery par la séquence : Récupération des pilotes des matériels, Réinstallation de Windows.
