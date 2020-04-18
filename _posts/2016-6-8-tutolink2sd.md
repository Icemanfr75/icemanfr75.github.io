---
layout: post
title: Tuto - Avoir plus de place pour ses applications sur son smartphone
category: tuto
tags: android, link2sd, root, Tutoriel
---
**Après avoir réussi à Rooter votre smartphone préféré (là encore je conseille de faire un tour sur <a href="http://www.phonandroid.com/">Phonandroid</a>), vous vous apercevez que vous êtes à l'étroit malgré les 8 ou 16Go promis par la notice. Car malgré une généreuse carte SD supplémentaire, les applications ne se déplacent pas toujours dessus. Les 16go devenus déjà 10 par l'entremise d'Android, deviennent limités pour utiliser plusieurs jeux premiums en plus de quelques applications. Mais il y a une solution.**

Il faut rappeler que cet état de fait est à la fois dû à Google mais aussi aux constructeurs de téléphones qui brident des fonctions et aussi aux développeurs qui empèchent l'utlisation de l'App2SD (mettre les données de l'application sur la carte SD) sur leur application. Ainsi les 3Go de Real Racing refusent obstinément d'aller sur la carte SD. Vous allez me dire qu'il en restera 7...mais avec des jeux premiums de plus en plus avides de place, ça commence à filer vite (Real Racing en faisait 1,2Go à sa première version il y a deux ans).

La vie est bien faite car cette solution s'adresse à des utilisateurs expérimentés. Et comme il faut déjà un téléphone rooté, ça veut dire que l'utilisateur en a déjà chié pour cela. Donc il a le droit d'utiliser .... Link2SD ! Je l'utilise sur mes téléphones depuis Android 2.1 et ça a toujours fonctionné. Sauf qu'il faut réfléchir à la place que l'on va laisser sur la carte SD pour ses applications. Il va falloir en effet partitionner cette petite chose en 2 : La première partition en FAT32 sera pour les documents, la musique, les vidéos.... La seconde en format EXT4 sera pour les applications. Pour faire cela, vous avez le choix des armes : Gparted sous linux ou bien un logiciel comme<span style="text-decoration:underline;"><a href="http://www.partitionwizard.com/"> Minitool partition Wizard</a></span> sous Windows (à condition d'être admin du PC).

Avant toute chose, vous devez déjà arrêter le smartphone, extraire votre carte SD et la mettre dans l'adaptateur fourni avec pour qu'elle soit lue sur le PC. **Si vous aviez des documents dessus, transférez les alors sur le disque dur du pc**. Lancez votre utilitaire et supprimez la partition de votre carte SD (ne vous trompez pas de disque)....Ensuite vous créez une partition primaire FAT32, puis une autre partition primaire EXT4 de la taille que vous avez laissé. Par exemple pour une 64Go, vous pouvez mettre 40 pour les données et le reste pour les applications. Appliquez les changements (ça prend du temps....). Ensuite vous pouvez copier à nouveau vos documents sur la partition FAT32.

Une fois cela fait, enlevez la carte, remettez là dans le smartphone et redémarrer le. Allez dans votre playstore préféré et téléchargez Link2SD. Il existe une version Plus qui permet plus de transferts pour 1,99€, mais il faut déjà installer la version normale. Une fois l'installation faite, il faut lancer Link2SD et il va demander quel format de partition vous utilisez : Répondez EXT4 et redémarrez le téléphone une nouvelle fois. Voilà c'est fait vous êtes prêts à récupérer des Go de données ! Au passage, je vous conseille de conserver la sauvegarde de votre SD sur le disque dur de votre PC.

Alors maintenant** il va falloir comprendre l'application**. Quand elle parle de "lier à la carte SD", il faut comprendre transfert. Ne pas confondre avec le transfert dit "App2SD" présent sur Android 5.0 et qui fonctionne aléatoirement. Voilà d'abord la fenêtre de Link2SD telle qu'elle apparaît :

<img class="wp-image-1387 alignleft" src="https://cheziceman.files.wordpress.com/2016/05/screenshot_2016-05-15-15-43-15.png?w=576" alt="screenshot_2016-05-15-15-43-15.png" width="213" height="449" />

Ici on voit des applications avec un message orange en dessous (lié-carte SD). Mais au début vous n'aurez pas ce message. En haut à droite vous avec trois icônes. Les trois traits en triangle inversé permettent de filtrer. Sélectionnez la rubrique "Déplaçable", ça évite les erreurs.  A droite de cet icône, il y a celui de tri. Sélectionnez "Taille Totale", tout en bas de la liste.

Je vous déconseille de vous occuper des applications de moins de 50Mo de toute façon. Dans l'exemple ci-contre, j'ai pris trois grosses applications qui mettraient à genoux bien des téléphones d'entrée de gamme. On va voir comment les déplacer maintenant. Je vous conseille de ne pas trop vous attarder sur les applications que vous testez quelques temps. Concentrez vous sur les applications que vous allez garder, ça évite de polluer la SD avec des données temporaires.

Appuyez sur la première d'entre elle maintenant . Vous allez avoir une fenêtre ressemblant à celle ci contre.

<img class="size-full wp-image-1386 alignright" src="https://cheziceman.files.wordpress.com/2016/05/screenshot_2016-05-15-15-43-33-e1463320275699.png" alt="screenshot_2016-05-15-15-43-33.png" width="281" height="500" />

L'application fait 186 Mo ici mais il y a 120MO de données. On va descendre un peu dans la fenêtre pour mieux voir les options proposées.

On voit que dans la case orange, il n'y a rien pour l'instant. On parle de "Lier à la carte SD" et cela ne concernera que les données de la rubrique App, pour l'instant. Dans la version normale de Link2SD, vous n'avez accès qu'à cette zone. Pour faire plus, il faudra penser à la version .... Plus.

Donc en dessous nous avons quoi ?

<img class="size-full wp-image-1388 alignleft" src="https://cheziceman.files.wordpress.com/2016/05/screenshot_2016-05-15-15-43-42-e1463320679167.png" alt="screenshot_2016-05-15-15-43-42.png" width="281" height="500" />

Obb est souvent la rubrique la plus utilisée. Son nom c'est Opaque Binary Blob file, officiellement mais je vous passe <a href="https://en.wikipedia.org/wiki/Opaque_binary_blob">les détails</a>. Vous pouvez "lier" aussi ces fichiers volumineux mais avant de faire cela, assurez vous d'avoir un téléphone bien chargé et de ne pas faire d'interruption pendant le transfert (évitez de brancher le chargeur, on ne sait jamais). Il va vous demander dans quelle partition vous souhaitez mettre ces données. Choisissez la "seconde partition", celle en ext4.

Dans le coin à droite, vous avez les habituels trois petits points du menu de l'application. Revenez sur la page principale de Link2SD, allez dans ce menu et faites Info-Stockage. Vous verrez votre carte SD avec le taux d'utilisation, sa partition EXT4 (invisible du système android)  etc etc... Normalement, votre mémoire interne a augmenté de beaucoup et si vous aviez un message vous prévenant que vous consommiez déjà 75% de l'espace, il va disparaître.

MAIS... il peut y avoir des problèmes lors de désinstallations et réinstallations d'applications. Une solution peut être d'utiliser une application comme <span style="text-decoration:underline;">SD Maid</span> mais avec précautions. Une fois que vous avez suffisamment pris en main tout ça, je conseille de faire une belle réinstallation en propre de votre téléphone avec un beau root tout neuf et un Link2SD aussi propre. Ca évite les ennuis pour un moment. Et surtout, on ne le répète jamais assez : Sauvegardez votre carte SD avant toute intervention.

Accessoirement, cette manipulation permet de prolonger la vie d'un téléphone de beaucoup. Bye bye obsolescence programmée ? ....pas sûr quand les éditeurs suppriment les versions de leurs applications pour Android 4.4 ou 5.0.
