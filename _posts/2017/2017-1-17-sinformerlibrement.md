---
layout: post
title: Tuto - 3 outils simples pour s'informer librement 
category: tuto
tags: android, flux rss, information, iOS, mobile, RSS, tutoriel, 
---
**Pour qui veut rester informé sur différents sujets, ou faire de la veille technologique, il y a bien des moyens de le faire. Mais si on veut faire sans les réseaux sociaux ou la lecture régulière d'un site, une solution sort rapidement du lot : Le bon vieux flux RSS.**

N'importe quel blog wordpress en crée un par défaut. Les grands médias en possèdent au moins un, voir des thématiques. Même les sites de piratage en ont... Je ne vais pas vous saouler avec <span style="text-decoration:underline;">les détails du rich site summary ou comment créer le sien (j'avais utilisé <span style="text-decoration:underline;"><a href="https://www.shaarli.fr/redirect.php">Shaarli</a>, par exemple par le passé). Disons en résumé que c'est un format qui permet d'avoir les liens des articles avec un extrait plus ou moins long de l'article. Le but ,ici, est de donner deux solutions accessibles à n'importe qui sur n'importe quoi (mobile ou fixe), sans auto-hébergement. Il s'agit donc de trouver des agrégateurs de flux (c'est comme ça que ça s'appelle).

Si vous avez un blog wordpress, autohébergé ou non, vous utilisez peut-être l'**application Wordpress** sur votre mobile. A l'intérieur, il y a ce qu'on appelle le Wordpress reader, qui reprend les blogs wordpress auxquels vous êtes abonnés sur un compte wordpress, le même que vous utilisez peut-être pour commenter ici même. Et bien dans cette interface de reader, sur un pc fixe, on peut intégrer n'importe quel flux RSS. Il suffit de taper l'adresse du flux et de faire ajouter. Mieux encore, on peut intégrer ce qu'on appelle le fichier OPML, pour <span style="text-decoration:underline;"><a href="https://fr.wikipedia.org/wiki/Outline_Processor_Markup_Language">Outline Processor Markup Language</a>. On comprend pourquoi c'est abrégé, hein. Ce n'est en fait qu'un fichier XML, un langage à balise qui permet l'import et l'export de ses flux RSS entre les plateformes. Cela permet par exemple de passer chez des plateformes propriétaires, sur des agrégateurs mobiles, etc....

Au passage, je vous conseille de garder régulièrement une sauvegarde de vos fichiers OMPL bien au chaud chez vous. Ca permet d'éviter des mauvaises surprises, genre fermeture de service, piratage de compte, etc... Sous le wordpress reader, il suffit d'aller dans Gérer ses abonnements (le menu de gauche) et de faire Exporter. <span style="color:#ff0000;">Par contre, à l'export, Wordpress modifie l'opml à sa sauce (ce qu'on peut corriger en éditant le fichier) ! Revers de la médaille de ce reader, il considère que nos abonnements sont partageables, par exemple à travers un widget du blog. Wordpress affiche donc des stats sur le nombre d'abonnés à un flux. Cela me dérange quelque peu. D'autre part, le flux ne se réactualise pas périodiquement et c'est lorsque l'on ouvre le reader que wordpress va interroger les flux et les mettre à jour. Lorsqu'on en a beaucoup, ça prend quelques minutes. Evidemment, ça évite de surcharger les serveurs par des requêtes régulières. Mais on risque aussi de rater des informations.

Alors, il existe une autre solution labelisée Framasoft : **<span style="text-decoration:underline;"><a href="https://framanews.org">Framanews</a>**. Il s'agit d'une instance d'un produit libre baptisé Tiny Tiny RSS (TTRSS). Evidemment, si vous maîtrisez l'autohébergement, vous pouvez avoir aussi votre propre instance ou un autre produit similaire. Car framanews n'est là que pour dépanner, limité à 100 flux et à une bonne poignée d'utilisateurs, ce qui est largement suffisant. Si vous ne l'utilisez pas pendant 3 mois, Framasoft vous demandera gentiment de laisser la place aux autres (j'ai laissé ma place). Vous allez alors me demander pourquoi Framanews plutôt que  Feedly ou encore Feedreader online? Tout simplement parce que les possibilités d'export et le partage des données n'est pas toujours clair . Certains intègrent la possibilité de s'enregistrer avec son identifiant facebook ou google, ce qui est une très mauvaise idée. Ce qui est intéressant avec Framanews, malgré une interface un peu toufue, c'est que cela initie à un produit qu'on peut autohéberger plutôt simplement. Les tutoriels sur le sujet sont légion et framasoft + la communauté d'utilisateurs sont là.

<img class="aligncenter size-medium wp-image-8290" src="https://cheziceman.files.wordpress.com/2016/12/framenws.png?w=300" alt="framenws" width="300" height="98" />

Comme un agrégateur classique, le serveur va récupérer périodiquement les flux, ce qui permet d'être au courant de tout, sur tout, partout. Car TTRSS est aussi compatible mobile/tablette. Et ne me dites pas que vous avez besoin de notifications pour apprendre qu'Angelina Jolie est avec Johnny Depp (quoi, vous ne saviez pas ???). Le push est totalement inutile car ce que vous apprendrez n'est qu'une dépèche rédigée sans aucun recul sur les faits.

Enfin, il existe **<span style="text-decoration:underline;"><a href="https://theoldreader.com/">The OldReader</a>,** un site qui dispose d'une solution **propriétaire** avec une API le rendant compatible avec pas mal de clients mobiles. Il est aussi tout à fait compatible avec une utilisation mobile. Problème, si TheOldReader ne pompe pas forcément nos données, il crée un profil comme pour Wordpress où nous partageons nos flux avec les autres. Mais il n'est pas possible pour un utilisateur de regarder les flux que suit un utilisateur qui n'est pas un "ami". Le produit est donc simple, un peu l'intermédiaire entre les deux produits vus au dessus et surtout il permet d'exporter son fichier OPML de manière fiable pour passer ultérieurement à une solution autohébergée. C'est sans doute le plus accessible au débutant, selon moi, sans semer trop de données, même si dans sa version gratuite, il ne met pas à jour tous les flux assez souvent.

Pour **ajouter les flux,** c'est très simple. Si suffit souvent de guetter l'icône suivante :

<img class=" alignleft" src="http://icons.iconarchive.com/icons/sicons/basic-round-social/512/rss-icon.png" alt="" width="348" height="351" />

Sinon, l'url principale peut parfois suffire. Avec quelques adresses bien choisies, en évitant les redondances, on arrive rapidement à avoir suffisamment d'information pour son temps de cerveau disponible. Vous oublierez rapidement Google News, Flipboard ou New Republic, ces sites et applications qui orientent et filtrent les informations avec plus ou moins de pertinence. Vous pourrez tout à fait mêler L'Humanité avec le Figaro et son alter égo parodique. Je vous ai même dit comment intégrer des <span style="text-decoration:underline;"><a href="https://cheziceman.wordpress.com/2016/11/01/tuto-instagram-sans-instagram/">comptes instagram</a>...

Alors maintenant c'est à vous de jouer avec ces trois produits simple d'accès et qui vont vous permettre de mieux choisir votre information, de la maîtriser, avant peut être d'héberger votre propre solution.

