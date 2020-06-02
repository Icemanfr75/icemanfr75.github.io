---
layout: post
title: Tuto - Gérer ses mots de passe
category: tuto
tags: tuto, hygiène numérique, sécurité, informatique, geek, web, 
---

**Pendant longtemps, j’ai évité ce sujet, trouvant cela inutile parce que j’avais le tort de ne mettre que des variantes de mots de passe faciles à se souvenir. Mais voilà, le monde numérique est devenu plus dangereux et on doit avoir des mots de passe différents pour chaque activité, chaque site. Et là, je me suis retrouvé avec une, que dis-je… des centaines de mots de passe.**

**Pourquoi ?**

Pourquoi plusieurs mots de passe déjà ? Parce qu’il suffit d’une faille quelque part pour qu’on trouve votre correspondance mot de passe identifiant et qu’ensuite on puisse faire tout et n’importe quoi. Nombreux sont les sites à encore stocker des mots de passe sans chiffrement et c’est très dangereux. Dans ma longue quête pour optimiser tout cela, j’ai repris un par un tous les sites que j’avais enregistré et j’en ai trouvé environ 5% qui posaient des problèmes au premier abord. En creusant, ça doit être bien pire.

![image1](https://cheziceman.files.wordpress.com/2020/05/password-hacking.jpg)

*derrière le code, des mots de passe*

Pourquoi les gérer alors ? Parce que cela permet d’éviter des redondances, des oublis. Cela permet d’avoir une vision de la robustesse de ces mots de passe. Et puis les gestionnaires de mots de passe permettent une fonction dont nous sommes incapables : Générer des mots de passe aléatoires. Pour tout vous dire, dans ma boîte, il y a obligation de changer tous les trimestres son mot de passe, qui ne doit comporter aucun mot se rapportant à nous, notre activité, ou au mois courant, qui doit avoir des minuscules, des majuscules, des chiffres, des caractères spéciaux. Ils ont limité cela à un certain nombre de caractère tout de même, mais on doit se creuser la cervelle car il ne doit pas y avoir de partie commune avec un précédent. Je vous ai résumé là, en fait, une des bonnes pratiques d’hygiène numérique. Je suis parti pour ma part de plusieurs centaines de mots de passe enregistrés pour arriver à une petite centaine après gestion et modification et parfois …suppression de comptes

**Les navigateurs et leurs comptes**

La première solution qui vient à l’esprit, c’est d’utiliser les fonctionnalités d’enregistrement des navigateurs. Chrome, Firefox, Opera ou même ceux des constructeurs de smartphone qui proposent cela. Si vous n’utilisez pas de compte google, opera, vivaldi, firefox, samsung, xiaomi,…(ce que j’aurai tendance à recommander), cela restera en local et vous n’avez aucune synchronisation avec les autres terminaux que vous utilisez. On trouve vite des limites à cela donc on utilise alors la fonction de synchronisation, la même qui met à l’abri vos favoris, parfois vos contacts, votre agenda…Selon les cas, c’est plus ou moins bien protégé, chiffré mais là encore, il suffit que l’on mette la main sur un de vos terminaux pour accéder à un export de ces mots de passe dans les options du navigateur. Bye bye la confidentialité. Il est possible de mettre parfois des mots de passe « maître », comme un gestionnaire de mot de passe qu’on appelle aussi Coffre-fort ou chambre-forte pour reprendre l’acronyme anglais « Vault ». Lors de l’enregistrement sur les navigateurs il n’est pas possible de mettre un nom particulier à l’enregistrement, ce qui est pratique pour faire la différence entre les redondances, des comptes multiples. La gestion reste limitée à l’intérieur du navigateur pour faire son tri périodique.

![image2](https://cheziceman.files.wordpress.com/2020/05/mdp5.jpg)

*L’interface d’Opera*

**Les coffres-forts**

Les coffres-forts se présentent selon le principe du client-serveur. Le serveur stocke votre base de données (en général un fichier chiffré) et donne l’accès à des clients sur les différents terminaux que vous possédez à l’aide d’une adresse, d’un login utilisateur et d’un mot de passe « maître ». Les clients sont soient des applications (logiciel linux, windows, android, iOS), soient des extensions aux navigateurs. Autant vous dire que les navigateurs constructeurs ne sont pas pris en compte donc il vaut mieux utiliser du classique comme firefox, chromium, opera, vivaldi…Je n’ai pas pu tester sur safari et iOS, mon banquier ne veut pas. Pour opera il faut parfois utiliser une extension qui permet d’utiliser les extensions chrome mais j’y reviendrai.

Parmi toutes les solutions du marché, il y a du libre, du open-source, du gratuit, du payant selon le principe de l’abonnement mensuel ou annuel. En bon libriste, j’ai d’abord commencé par des solutions libres et j’ai regardé ce que faisaient les autres, les noms qui ressortent le plus. J’ai donc regardé Passman qui est intégré à Nextcloud, Keepass et ses nombreuses variantes. Je suis ensuite allé voir Bitwarden qui dispose d’un fork que l’on peut installer chez soi. Et j’aurai pu tester aussi Lastpass pour ce qui est des solutions payantes et tant d’autres. Pour Keepass, Passman et Bitwarden, on peut faire de l’auto-hébergement du serveur mais il vaut évidemment mieux avoir quelques compétences en sécurité réseau pour éviter la bévue. Je vous préviens, je ne vais pas me faire de copains dans le choix que j’ai fait donc il faut que j’explique ce que je voulais faire.

![image3](https://cheziceman.files.wordpress.com/2020/05/mdp3.jpg)

*L’interface de Passman dans le navigateur*

**Le Cahier des charges**

N’étant jamais fixé sur un navigateur en particulier, je veux que la solution fonctionne sur tous mes ordinateurs quelque soit le navigateur utilisé. Je veux aussi que ça fonctionne sur mon smartphone android. Je veux que ça détecte automatiquement qu’on me demande un mot de passe et que ça me propose de remplir les champs de saisie. Je veux pouvoir l’éditer de n’importe quel terminal aussi. Mais je veux aussi être à l’abri des évolutions logiciels de terminaux donc qu’il y ait du développement derrière. Vous allez voir que ça coince… Enfin, je veux que la solution reste accessible au plus grand nombre, parce que la sécurité est l’affaire de tous.

![image4](https://cheziceman.files.wordpress.com/2020/05/mdp4.jpg)

*Simple, Passman dans Nextcloud*

**Passman**

![image5](https://cheziceman.files.wordpress.com/2020/05/mdp1.jpg)

*Intégration de Passman sur Opera*

Je l’utilisais depuis 1 an sur mon instance Nextcloud et ça marchait bien avec Firefox. Avec Opera, il faut ruser en prenant d’abord l’extension pour les extensions chrome puis aller dans le chrome webstore pour l’installer. Evidemment il faut une instance Nextcloud pour faire le serveur et sur mon instance Zaclys ça se passe très bien, en dehors des temps de réponse. Le problème est sur Android. Il y a bien une application Passman mais elle reste quasiment en Alpha, freeze ou plante constamment. Je suis allé voir sur le github et ça ne progresse plus beaucoup donc pour moi, c’est une solution moribonde. C’est dommage car les possibilités sont là, notamment le classement des items selon la robustesse du mot de passe, les étiquettes…. Il y a autre chose qui fonctionne mal, c’est la suppression des items qui sont dans la corbeille. Aucun choix multiple (demandé depuis quelques années) et on se retrouve à exporter les suppressions lorsque l’on veut faire une sauvegarde de l’export. C’est un peu lent à réagir en plus donc j’ai cherché autre chose.

![image6](https://cheziceman.files.wordpress.com/2020/05/mdp2.jpg)

*Ce qu’il faut rajouter avant d’intégrer Passman sur Opera*

**Keepass**

Genma parlait souvent de Keepass, ou plutôt de Keepass X, non Keepass XC, parfois de Keepass 2. Oui, il y a des tonnes de fork, de variantes, de clients compatibles. Au moins ça vit encore… C’est compatible Nextcloud, il suffit d’héberger son fichier sur son serveur et d’aller le chercher avec le client de chaque terminal. Sur un PC, il y a donc un logiciel de gestion ce qui est assez pratique pour faire du ménage. Par contre, pour la détection automatique, ça ne le fait pas trop, donc si ouvrir, cherche, copier, coller vous rebute, passez votre chemin. Certaines interfaces m’ont ramené 15 ans en arrière.

![image7](https://cheziceman.files.wordpress.com/2020/05/mdp6.jpg)

*Simple mais oldschool*

Heureusement, le fork KeepassXC est un peu plus moderne. J’ai pu par exemple y importer mes bases en CSV, que ça soit du passman ou du Bitwarden. Il suffit juste de lui dire quels champs correspondent à quoi. Le fichier .kpdx peut être placé simplement dans un répertoire de votre instance Nextcloud. L’application Keepass2android s’y connecte ensuite avec l’adresse en HTTPS, le mot de passe et le login du Nextcloud. Je dois dire que l’application est beaucoup moins intuitive que d’autres et que la détection automatique dans les navigateurs d’un smartphone ne coule pas de source. Pas plus d’ailleurs avec le plugin chrome qui ne fonctionne pas bien sur Opera. Donc je ne peux pas conseiller à quelqu’un de débutant qui n’est pas prêt à suivre scrupuleusement des instructions. Débutant qui n’aura pas forcément d’instance Nextcloud, d’ailleurs, même si ça passe aussi sur des outils plus « courants » (dropbox, box…). Donc j’ai cherché plus simple et avec tous les imports exports essayés, j’ai vu souvent revenir le nom de…

![image8](https://cheziceman.files.wordpress.com/2020/05/mdp8.jpg)

*KeepassXC*

**Bitwarden**

Bitwarden n’est pas libre mais peut le devenir avec sa variante Bitwarden_RS, sinon il est juste open-source. Bitwarden est disponible en une version gratuite suffisamment riche pour être suffisante. La version payante à 10 $/an ce qui est aussi très accessible. On a une interface assez simple, du choix multiple sur l’interface web même s’il faut parfois entrer dans chaque item pour le manipuler. Beaucoup de format d’importation aussi ce qui permet de prendre son export de navigateur ou d’une autre solution (JSON pour Passman, par exemple). L’application Android est efficace, fonctionnant en tâche de fond ou sur demande pour remplir les champs. Une extension est disponibles sur tous les grands navigateurs du marché. Et on peut même héberger son serveur, soit en payant une licence, soit en utilisant le fork Bitwarden_RS. Je n’ai pas essayé mais ça me laisse au moins cette possibilité plus tard, de même que l’export en CSV qui sera lisible ailleurs. On a la gestion des authentification à double facteur en plus (surtout en compte premium). ( le récent Cozy Pass est un fork de bitwarden mais manque encore de finition et de fonctions )

![image9](https://cheziceman.files.wordpress.com/2020/05/mdp7.jpg)

*L’interface web de Bitwarden*

**Le Choix de l’outil**

Donc j’ai opté pour l’instant pour Bitwarden qui reste fiable dans ce que j’en ai vu. Je fais aussi un export régulier de ma base sur un support offline. Je n’ai donc pas eu envie de me lancer dans toutes les autres solutions payantes du marché qui permettent parfois des comptes limités en gratuit. Tout le monde n’aura pas forcément les même besoins que moi, plus ou moins riches. Je n’ai pas mis de mots de passe d’applications, de logiciels, de carte bleue, j’ai encore un cerveau assez performant pour cela. Car le risque à un moment est de ne se reposer que sur cela. Pour moi, cet outil est là pour me venir au secours si je ne retrouve pas mon mot de passe. J’ai trouvé ma propre technique de création de mots de passe qui pour l’instant résiste efficacement au temps. Et pour les plus critiques des mots de passe, je passe effectivement par de l’aléatoire, plus difficile à retenir.

Je n’ai pas retenu Buttercup qui semble plutôt pas mal, parce qu’il n’y a pas d’extension native pour Vivaldi, Opera. Je n’ai pas non plus pris Lastpass, autre solution commerciale comme Dashlane ou 1password parce que je n’ai pas vu de plus majeur par rapport à ce que j’ai trouvé ici. Je reste ouvert pour le futur avec cette possibilité de tout héberger « chez moi », si je le veux. Je pourrais conseiller KeepassXC pour les plus spécialistes qui ont les compétences pour héberger une instance et configurer les outils. La solution est fiable, avec une communauté de développement (même si ça part dans tous les sens) et un standard reconnu.

**Et ensuite**

J’ai donc fait un gros ménage qui a fait diminuer de 75% ma base de données. J’ai pris le temps de changer tous les mots de passe faible sur chaque site, tous les mots de passe les plus critiques aussi. Il faut éventuellement identifier par étiquette ou dossier ceux qui seront à reprendre souvent. La périodicité de révision n’est parfois pas du luxe, surtout si on détecte une faille. Il ne faut pas hésiter à supprimer les comptes superflus sur les sites qui ne respectent pas certaines règles de sécurité. En changeant les mots de passe, on s’en aperçoit assez vite. Il est très rare qu’il y ait une vérification / validation solide. Sinon on s’en aperçoit lorsqu’on utilise la fonction de récupération de mot de passe. Pour les comptes email utilisés, faites aussi attention selon la criticité du site. Je reste avec ma logique :

- Site officiel, administratif, institutionnel : Un compte mail sécurisé
- Site de boutique : Un compte bien équipé en antispam
- Sites personnels : Un compte … personnel dédié à ça.

A chacun de voir pour son réglage, sa capacité à réviser régulièrement ses Mots de passe. C’est un peu de boulot au début mais une fois bien réglé, c’est juste du confort et de la sécurité.

[la video](https://youtu.be/B32yjbCSVpU)


