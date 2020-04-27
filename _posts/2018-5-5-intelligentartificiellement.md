---
layout: post
title: Blog-tuto - Et si j'étais intelligent... artificiellement
category: geek, tuto
tags: blog, méthode de travail, Réflexion, travail, tutoriel, 
---
**Comme beaucoup de personnes (...ou pas), j'ai lu les propositions du <a href="http://www.enseignementsup-recherche.gouv.fr/cid128577/www.enseignementsup-recherche.gouv.fr/cid128577/rapport-de-cedric-villani-donner-un-sens-a-l-intelligence-artificielle-ia.html">rapport Villani</a> sur l'intelligence artificielle. Et comme je n'attends pas ce genre de rapport pour me poser des questions sur ma propre activité, j'ai regardé ce que je pouvais améliorer. L'occasion de faire des tests et de clôturer enfin des expériences.**

Je sais que j'ai fait grincer le bec de mon <a class="mw-redirect" title="" href="https://fr.wikipedia.org/wiki/Sph%C3%A9niscid%C3%A9">sphéniscidé</a> parisien préféré, ces derniers temps avec mes robotisations, mes multiples comptes qui se recopiaient. Je détaillerai tout ça dans un autre billet. D'abord parlons de ce que peut apporter un peu d'intelligence artificielle dans la vie de tous les jours.

Cela fait des années que j'améliore petit à petit tous mes outils de dépouillement d'essais, de calcul pour me faciliter la tâche. Je n'aime pas réinventer les choses qui existent mais les améliorer, si (principe du <a href="https://fr.wikipedia.org/wiki/Kaizen">Kaizen</a>). Ainsi, il est très facile de commencer par traiter des données aussi simples que ses comptes personnels pour comprendre l'exemple. Les banques fournissent des applications, ce qui indirectement, leur fait connaître notre vie, mais on peut faire la même chose très simplement en utilisant l'extraction des données du compte en <a href="https://fr.wikipedia.org/wiki/Comma-separated_values">CSV</a> et faire un simple copier-coller dans Excel/Calc pour avoir tous les bilans, les tris possibles en un seul clic et sans macro. Sur le même principe, j'ai évidemment des données d'une centrale d'acquisition qui passent à la moulinette, avec détection de différentes zones, recherche de l'équation de modélisation, correction des erreurs systématiques... Le temps que l'on va passer à mettre au point l'outil sera gagné très vite** si c'est une tâche répétitive et fastidieuse**. C'est donc là dessus qu'on devra focaliser ses efforts. (et j'ai passé encore des heures à ça, ces dernières semaines pour une nouvelle méthodologie d'essai)

Mais attention à ne pas tomber dans l'excès de zèle. Car plus on a de données, plus on veut faire de tableaux de bord et bilans que l'on mettra aussi du temps à compiler  et exploiter. Le but est bien d'**avoir une valeur ajoutée immédiate**. Si je reprends l'exemple des comptes bancaires, le but premier est de savoir si on dépense trop et sur quel poste. On peut donc se contenter de la visualisation du top des dépenses, par exemple et pas des graphiques dans tous les sens. On peut aussi rechercher les périodes critiques de l'année si on a déjà prévu les dépenses périodiques. Là encore, une petite réflexion préalable et après l'outil devient invisible...L'autre souci est de savoir comment on obtient les données. S'il fallait une heure pour récupérer correctement les données de mon compte bancaire, je ne le ferai pas. Mais il ne me faut que 2 minutes, donc ça va. Je connais d'autres outils qui demandent la participation de centaines de personnes avec un temps important pris dans la charge de travail. C'est de la connerie artificielle, à ce moment... voire réelle.

![image](https://cheziceman.files.wordpress.com/2018/04/applewatch.jpg)

*Intelligence superflue?*

L'intelligence artificielle, c'est aussi ce que nous avons déjà **au cœur de nos smartphones**. Mais comme nous les utilisons bien mal, nous ne le remarquons pas. Aujourd'hui, on peut avoir des fonctions pour couper et remettre le réseau de données, se mettre en mode nuit sans lumière bleue, aller chercher ses <a href="https://cheziceman.wordpress.com/2017/05/18/tuto-du-bon-usage-du-courrier-electronique/">mails</a> périodiquement, supprimer le superflu, trier dans des rubriques, rappeler ce qui est réellement important à faire au bon moment. On peut aussi faire des passerelles entre nos différents réseaux sociaux avec des automatisations comme ce que propose <a href="https://ifttt.com">IFTTT</a>, par exemple (j'y reviendrai prochainement). On a même des possibilités de filtre et de redirection sur des flux RSS avec d'autres outils afin de traiter des informations pour éviter d'être noyé. Les fonctions de calendrier avec rappel sont aussi des mines d'automatisations possibles du travail de groupe mais attention à ne pas en abuser  car la systématisation fait qu'on ne lira plus rien. C'est aussi ce qui nous énerve avec les notifications de toutes les applications, le push,... Ce que je bannis tout de suite sur mon smartphone. Je ne garde visible que ce qui me sert vraiment, je supprime les droits d'accès à toutes les applications qui n'en ont pas besoin, les démarrages automatiques. Ce travail qui peut vous prendre quelques heures, finira par vous en faire gagner à ne plus avoir le nez collé à chaque bip ou led allumée. D'ailleurs, un truc sympa pour savoir l'heure a été inventé il y a très longtemps ... La montre ! Pas besoin de l'avoir dans un coin de votre vue non plus.

L'intelligence artificielle nécessite une intelligence réelle, celle de faire un tri dans ses activités **entre l'essentiel et le superflu**. J'entendais des juristes et avocats parler de cette intelligence dans la recherche de documentation, les lourdeurs administratives. Ce sont des activités essentielles mais lourdes en temps et qui ne permettent pas de se concentrer sur la construction d'un dossier, la plaidoirie, etc. De la même manière, lorsque l'on gère plusieurs fichiers en parallèles qu'il serait impossible de réunir en un seul (car trop lourd en poids et plusieurs intervenants en même temps), on peut avoir envie d'en extraire un tableau de bord synthétique, de rechercher des cas particuliers, au lieu d'avoir périodiquement à analyser chacun de ces fichiers. Là encore, ce sont des requêtes simples à base de "conditions si" multicritères et de "alors". On s'aperçoit que beaucoup de cette "intelligence" passe justement dans la détection de ces "Si". Prévoir les cas les plus tordus fait partie de beaucoup de nos activités. Cela va des formulaires de saisie où on évite l'erreur par un contrôle, un formatage, jusqu'à de la surveillance d'installation pour éviter une casse. Il y a ainsi une intelligence discrète dans les smartphones sur la température du processeur ce qui crée des baisses de fréquence si c'est dépassé ou si elle n'est pas nécessaire. Les aides à la conduite sont aussi avec des Si sur le résultat de mesure de beaucoup de capteurs combinés.

![image](https://upload.wikimedia.org/wikipedia/commons/a/ab/Botticelli_ChartOfDantesHell.jpg)

*Carte de l'Enfer de <a href="https://commons.wikimedia.org/wiki/File:Botticelli_ChartOfDantesHell.jpg">Sandro Botticelli</a>*

Mais **la faiblesse humaine** est de faire tellement confiance à cette intelligence que l'on oublie de l'être, intelligent. C'est ce qui est arrivé aux conducteurs de prototypes de voiture autonome, par exemple. C'est ce qui arrive quand on conduit trop vite en courbe en pensant que l'<a href="https://fr.wikipedia.org/wiki/%C3%89lectrostabilisateur_programm%C3%A9">ESP</a> et l'ABS nous sauverons. C'est ce qui arrive en suivant toutes les indications du GPS, sans regarder vraiment les indications sur la route. C'est ce que l'on fait en prenant les photographies numériques à la volée sans penser aux réglages, parce que derrière on fait confiance à la machine pour corriger. La faiblesse est de croire que toutes nos erreurs seront rattrapées par quelqu'un ou... Quelque chose. Mais le quelque chose dépend lui même d'autres facteurs. Le meilleur pilote automatique d'avion peut avoir des cas qu'il ne saura pas gérer. Le risque zéro n'existe pas. Et la première des intelligences, bien réelle, cette fois, c'est d'analyser les risques. Une démarche bien connue mais pas assez bien formalisée. Je ne me vois pas l'aborder ici, mais il doit bien y avoir des vidéos sur le sujet, puisqu'aujourd'hui on pense MOOC.

Il ne faut pas oublier que derrière l'intelligence artificielle, il reste des humains avec des failles, des buts et donc des choix à faire. Aujourd'hui on parle d'algorithmes pour gérer plein de choses et surtout nos erreurs. Comme le rappelait Cyrille il y a quelques semaines, le problème reste bien l'humain entre tout ça qui va très vite oublier ce que peut faire la machine. On a vu cela aussi dans les finances avec l'intelligence artificielle dans les spéculations boursières. Les humains ne comprennent plus ce qu'il se passe, paniquent et finissent par couper la machine lorsqu'il est trop tard. Tout ça étant dit, on peut quand même vivre très normalement sans penser à tous les risques et en étant intelligent sans artifices. Je crois que mon ami Tom l'a bien compris, là.

[video](https://www.youtube.com/watch?v=G2UVsyVLLcE)

Et puis donc j'ai fini de faire le tour de Twitter après 5 mois. Le compte reste présent mais je ne suis (du verbe suivre...) plus vraiment personne et il n'y a plus rien à suivre. Pas de problème de clash, je sais m'en prémunir. J'ai plus de problème de publicités (je bloque toutes les sources) et de Hashtags sponsorisés, finalement et ça montre la dérive de ce réseau qui est devenu<a href="https://m.slashdot.org/story/340313"> un autre Facebook</a> avec les mêmes travers. Je suis aussi allé voir Mastodon, ce réseau libre équivalent auquel je ne croyais pas quand il faisait le buzz. J'avais raison car il ne se passe plus grand-chose. La plupart des comptes sont des robots, des réplications de twitter ou des gens qui parlent de cryptomonnaies. Peu intéressant donc en tout cas pas assez pour y passer du temps, et les statistiques qui augmentent tiennent pour beaucoup à ces intelligences artificielles pour robotiser les posts. Pas de vrai contenu donc, pas de vrais commentaires ou si peu. Je deviens donc aussi un Bot de plus, pour ceux qui n'iront pas à l'adresse quelques lignes plus bas, et j'ai donc revu mes flux RSS dans cette même période. J'ai viré les flux d'auteurs de BD qui ont migrés sur Instagram, tant pis pour eux. J'ai privilégié des flux d'actualité "lents", ceux qui ne sont pas dans la réaction immédiate. Et j'utilise donc une fonction de partage de TheOldReader qui permet de créer son propre flux RSS. On y accède là : <a href="https://theoldreader.com/profile/iceman75">https://theoldreader.com/profile/iceman75</a>

Et puis je me suis attaqué au PC de madame et là, je n'ai pas été assez intelligent. J'aurais dû regarder les forums avant ... sur ce satané Dell XPS15 de 2011 avec cette horrible double carte graphique pour couronner le tout. Il y a véritablement un problème avec Grub avec les installations d'ubuntu et dérivés. Rien d'insoluble à priori mais je me suis demandé ce que j'oubliais dans les partitions pour que ça merde comme ça.... avant d'avoir simplement l'idée de chercher sur le net de constater que beaucoup d'autres avaient ce problème. Et <a href="https://www.blog-libre.org/2018/04/29/apprendre-comprendre/">Cascador</a> qui parle du problème d'apprendre et comprendre et d'avoir envie de comprendre, de savoir se mettre à la portée des autres. Je trouve que les installations graphiques ont raté le coche en masquant les problèmes et les explications possibles. Pour une fois que je passais par ce mode d'installation... Je serai plus intelligent la prochaine fois. En attendant, j'ai fait un sort <a href="https://forum.xda-developers.com/redmi-note-3/how-to/how-to-disable-google-apps-root-miui8-t3563192">aux Google Apps</a> qui restaient sur mon smartphone et j'ai mis du <a href="https://wiki.zaclys.com/index.php/Dégoogliser_votre_téléphone_Android">libre hébergé dedans</a>.... à suivre.