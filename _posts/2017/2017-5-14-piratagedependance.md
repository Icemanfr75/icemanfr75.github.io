---
layout: post
title: Piratage - Le jour où l'on découvrit notre dépendance...
category: tuto, geek
tags: Geekeries, internet, piratage, Réflexion, réseau, sécurité, tutoriel, 
---
**... A l'informatique et aux réseaux est arrivé Vendredi. Enfin, presque, car je ne suis pas sûr que tout le monde réalise les dangers, tant qu'il n'y a pas été confronté.**

Pour savoir de quoi je parle, un petit détour vers un article peut aider... en voici <a href="http://www.courrierinternational.com/article/securite-informatique-cyberattaque-une-tempete-planetaire">un</a>. On y voit que de l'opérateur réseau, au système de santé, en passant par un constructeur automobile ou un transporteur de colis, tout y est passé. Mais au lieu d'une classique attaque par déni de service (comme il y a eu cette semaine sur un noeud du réseau de la presse française, suffisamment stupide pour avoir un fournisseur de service unique), c'est passé par un ransomware qui s'est propagé d'une manière pas encore totalement identifiée. Un ransomware, pour faire simple, c'est un virus qui va vous empêcher d'accéder à vos fichiers et vous demander une rançon en échange. Celui ci, baptisé <a href="http://www.zataz.com/ransomware-wcry/">WCry,</a> serait apparu un peu avant début février, sans doute, et exploite une faille windows qui a été rapidement corrigée.

![image](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2017/wcryscreen.png)

Quand je vous dit que chiffrer ça peut aussi être mauvais...

Comme souvent, ce type d'attaque montre beaucoup de choses sur notre fonctionnement : On a toujours le problème de **la mise à jour** des systèmes d'exploitation (ici, c'est l'arrêt de support de Windows XP qui a signé l'arrêt de mort de PC bloqués sur cet OS pour cause d'applications spécifiques*), antivirus etc...  chez les utilisateurs et que les gestionnaires de parc se retrouvent à forcer dans ces cas extrèmes, plutôt que d'attendre le bon vouloir de l'utilisateur distrait (oui, ça peut prendre 1/2 h de notre temps de travail...). Il y a **le comportement à risque** de l'utilisateur qui fait n'importe quoi avec son ordinateur du boulot, va sur des sites dangereux, ou ouvre des pièces jointes douteuses. On a beau le dire, il y a toujours le syndrome du "c'est pas moi, c'est les autres". Mais ce ne sont que des causes immédiates. Il faut regarder en amont, ce à quoi notre ordinateur nous sert.

* Il nous sert déjà à nous connecter à un réseau. Coté entreprise, il sert à aller chercher des données sur un/des serveurs, à travailler sur ces fichiers, puis à les sauvegarder sur ces serveurs.
* Il nous sert à travailler localement sur une tâche, avec là encore des fichiers qui eux ne sont souvent pas sauvegardés
* Il nous sert à aller chercher des informations sur le réseau extérieur, Internet.
* Il nous sert à communiquer par différents biais (mail, messagerie instantanée, ...) en interne et externe.

Maintenant, imaginons que cet outil disparaisse.... **Est-on capable de continuer à travailler suffisamment longtemps pour laisser le temps de récupérer cet outil ? **La réponse montrée par cette infection de grande échelle est NON. Il faut regarder différents points :

* 1- A-t-on un autre ordinateur qui reste déconnecté de tout réseau et n'a jamais de transfert de fichier par clé USB?
* 2- A-t-on un autre ordinateur qui n'utilise pas le même système d'exploitation que les autres ?
* 3- A-t-on une copie de ses données utiles / locales sur un support non connecté.
* 4- A-t-on de quoi réinstaller ses logiciels indispensables (ou équivalents) ailleurs ?
* 5- Sait-on fonctionner sans le moindre support informatique ?
* 6- Les données sensibles sont-elles chiffrées ?

La question 5 peut paraître anachronique et évidemment ne pourra pas être applicable dans les professions de l'informatique. Pourtant, lorsque l'on lit qu'on ne sait pas identifier des bébés par des bracelets imprimés, on peut se poser ce genre de questions sur beaucoup de nos activités. Alors si vous n'avez coché que  2  ou moins de 2 de ces items, il faut vite agir. Dans ma boite, la gestion du système informatique répond à deux de ces items. Le reste est du domaine de l'utilisateur, pour l'instant.

* **Imaginons maintenant que ce soit le réseau électrique qui soit touché**....Est-on en mesure de fonctionner ? Evidemment non, aujourd'hui. La question que pose aussi cette attaque est de savoir comment sont protégés les moyens de production d'énergie, des centres névralgiques où l'on a agit souvent bien plus que chez les entreprises et services concernés aujourd'hui. Il y a donc des solutions et il ne faut pas céder à la panique en se disant que tout va tomber. Mais bon, qu'un réseau téléphonique soit si exposé, par contre, est un peu inquiétant, même s'il faut relativiser. Est-ce que toutes les télécommunications espagnoles ont sauté ? Non. Très récemment et localement, on a eu un r<a href="http://www.leveil.fr/puy-en-velay/internet-multimedia/2017/04/06/les-reseaux-sfr-et-bouygues-a-nouveau-fonctionnels_12354528.html">éseau mobile paralysé </a>en France, sans piratage. Quand c'est une panne <a href="http://www.leparisien.fr/high-tech/sfr-nouvelles-perturbations-sur-le-reseau-mobile-de-l-operateur-18-08-2014-4071719.php">nationale</a>, cela oblige l'état à de l' interventionnisme auprès de ces entreprises privées, bien que des services de l'état soient eux aussi touchés. L'interdépendance de tous les services est un fait. Mais vient aussi le problème de la **"cyberdépendance"**.

On cède aussi à la panique lorsque l'on n'a plus ses petits services habituels. On se croit par exemple à l'abri si on a mis ses données chez un prestataire de "cloud". Sauf qu'en cas de coupure réseau, de disparition de ce service pour cause de piratage, aurevoir les données.... Notre smartphone est souvent une clé pour rentrer dans nos données, une clé que l'on peut perdre bien plus facilement encore qu'un ordinateur. Les données qui y sont, sont donc à sauvegarder régulièrement de la même manière que ce que l'on fait avec un PC, puisqu'un smartphone EST un ordinateur. Et aujourd'hui avec un système dominant (Android), voir deux (iOS aux USA), l'exposition au piratage est particulièrement importante. Sauf qu'on peut revenir plus facilement à une activité sans son smartphone. On peut utiliser un téléphone classique pour cette activité. On peut se connecter à sa messagerie un peu plus tard et ailleurs (voir un tuto prochain sur le sujet des mails). On peut se diriger avec un GPS, une carte papier....On sait faire si on oublie ce moment de panique initial.

Cette attaque massive, qui se reproduira d'autres manières et de plus en plus souvent, nous impose de nous poser toutes ces bonnes questions. On peut être geek et savoir se passer de tous les gadgets informatiques et connectés. On le fait, enfin moi, quand on part en vacances. On peut s'imposer ces moments de pause pour regarder justement ce qu'il arriverait si .... C'est à ce moment que l'on s'aperçoit de ses erreurs et de ce que l'on doit parfois apprendre. ​Et à ceux qui me répondront "Auto hébergement", je répondrais qu'avant d'en passer là, il vaut mieux examiner l'utilisation des outils et l'accès aux outils disponibles, comme a pu le faire <a href="https://cyrille-borne.com/article4037/nextcloud-en-deux-coups-avec-snap-et-ubuntu-serveur">Cyrille ces derniers jours,</a> avec sa verve habituelle.

* : pour les applications spécifiques à un OS, on oublie trop souvent les possibilités offertes par la virtualisation, par <a href="https://www.virtualbox.org/wiki/Downloads">Virtual Box</a>, par exemple. J'ai utilisé ce principe pour une vieille chaine d'acquisition AOIP SAM 20 n'ayant plus de support de son constructeur.
