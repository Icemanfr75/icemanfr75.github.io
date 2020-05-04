---
layout: post
title: Tuto - Excel, Calc, ou Le tableur et ses pièges 
category: tuto
tags: bonnes pratiques, calc, excel, Geekeries, libre office, programmation, tableur, travail, tutoriel, 
---
**J'avoue tout : Le tableur reste mon outil préféré. J'y fais mes comptes, je modélise et traite des résultats de mesure dans mon travail, j'y ai aussi la saisie d'inventaires et de plannings.... L'outil à tout faire mais qui peut vite se révéler un cauchemar.**

Je ne vais pas passer du temps sur les basiques du fonctionnement d'un tableur mais parler de tout ce qui n'est pas dit mais vous facilitera la vie avec .... les autres. Car même si vous produisez des feuilles de calcul pour vos besoins propres et sans les échanger, pensez qu'un jour ou l'autre il y aura un changement de version, de système d'exploitation, ou carrément de logiciel. Vous avez peut-être utilisé Lotus 1-2-3, puis Microsoft Excel, puis Star Office, Open Office et maintenant Libre Office... ou autre. Et tout ça en moins de 20 ans.

<img class="aligncenter size-full wp-image-22483" src="https://cheziceman.files.wordpress.com/2018/03/oo3.png" alt="" width="632" height="282" />

**Les Calculs et les formules**

Je suis un fanatique des formules, souvent imbriquées mais le défaut de tout ça, c'est que ce n'est pas un code sous forme de listing. Cela veut dire qu'il faut laisser de quoi rendre cela compréhensible par celui qui passe derrière vous. Ca veut dire, par exemple avoir des zones clairement définies avec des petits "commentaires" qui expliquent le sens de la formule, en titre par exemple. Ou alors, ça peut être aussi **une feuille de mode d'emploi**, masquable, et qui aidera le "super utilisateur" de votre feuille de calcul. Et puis, on ne sait jamais, il peut y avoir des changements avec les formules aussi (par exemple les écarts-types....) ce qui nécessitera de comprendre ce que l'on a fait par le passé.

**Les Macros**

Je n'ai jamais été adepte des macros. Déjà parce que l'interface dans Excel m'a toujours rebuté mais en plus par philosophie pour ne pas être prisonnier d'un langage propriétaire et donc orienté Microsoft uniquement. Si les macros peuvent effectivement être très pratiques, il faut penser aux évolutions et aux personnes qui vont les utiliser. Donc ça veut dire impérativement commenter son code ou en laisser une documentation claire. Mais ce qui me fait tiquer sur les macros c'est que même avec une même famille de logiciel, on a eu des changements de langage et là, c'est vite la catastrophe dans l'optimisation du code. En pleine migration d'Office en ce moment, je vois ce que ça peut créer comme problèmes. Donc **pensez d'abord à faire simple.** 

**Les défauts de la mise en forme conditionnelle**

Il fut un temps où j'utilisais pas mal la mise en forme conditionnelle. Je le fais par exemple pour mes comptes personnels. J'ai des rubriques, des couleurs quand je dépasse des seuils, etc. Ca va, c'est figé mais** le problème**avec ce type de mise en forme arrive** lorsqu'on fait des insertions de colonnes et lignes**. Là, c'est la catastrophe car le tableur scinde tout ça en plusieurs mises en forme et ça allourdit considérablement le fichier et les calculs en tâche de fond. On réservera donc ce type de mise en forme pour une structure qui ne bouge pas.

**La saisie par liste déroulante**

**(ça concerne surtout Excel car Libre Office gère ça autrement)** Pour faciliter la saisie et éviter les fautes d'orthographe, pour avoir des tableaux croisés dynamiques qui fonctionnent bien, j'utilise la fonction de saisie par liste déroulante. Le problème est d'avoir le contenu de cette liste dans un endroit qui ne risque rien. Deux solutions : Une feuille à part que l'on va masquer, ou bien une zone de la feuille utilisée mais que l'on masquera aussi, avec une protection, si possible. Mais attention à ne pas mettre ça dans une zone susceptible d'avoir des insertions dans tous les sens. Par exemple pour une liste où on ajoutera des lignes, on ne mettra pas la zone de liste à droite ou à gauche du tableau mais au dessus.

**L'insertion et ses pièges**

L'insertion, ça parait hyper simple avec le bouton droit de la souris. Mais **ça commence à ne plus fonctionner dès qu'on a des formules dans les lignes ou colonnes**. Excel et ses copains ont beau être intelligents, ils ne peuvent pas deviner tout. Je conseille plutôt le duo : Insertion+copier-coller de la ligne du dessous...ou sinon le copier - insérer la ligne/colonne copiée. Il suffira de changer juste les quelques contenus différents et ça évitera de perdre des formules.

**Surveiller ses fichiers régulièrement**

Moi qui ai souvent des fichiers en partage avec une dizaine de personnes du service sur un serveur, je prends tous les jours un risque de perte de données. Pour éviter ça, je dispose déjà d'**un backup journalier au niveau serveur**et j'ai **gardé les modèles des fichiers**pour reprendre toutes les formules rapidement. Mais surtout je fais un tour régulièrement pour vérifier s'il n'y a pas des petits malins qui ont fait des insertions malheureuses, des suppressions, etc...Quand ça merde vraiment, on le sait très vite de toute façon. Bref, il faut se souvenir du mot "Sauvegarde", comme toujours.

**Le Copier-Coller dans un autre document**

Quand on a un tableau excel/Calc, il arrive souvent qu'on le colle dans un document Word/Write et qu'on envoie le tout à quelqu'un. Le problème est que parfois on colle TOUT le document, c'est à dire toutes les feuilles derrière et ça c'est dangereux. Il y a déjà la confidentialité des données, mais aussi la possibilité pour une personne mahonnête de retoucher vos données ensuite. Bref, pour ne pas être embêtés,** utilisez le "Collage spécial"**disponible dans le menu édition et collez une image du tableau ou un format qui ne contient que le tableau et rien d'autre.

<img class="aligncenter size-full wp-image-22480" src="https://cheziceman.files.wordpress.com/2018/03/collage-special.jpg" alt="" width="427" height="227" />

Et puis il y a évidemment le problème des images, comme dans les tableurs, que l'on peut régler avec ce petit menu:

<img class="aligncenter size-large wp-image-22481" src="https://cheziceman.files.wordpress.com/2018/03/compression.jpg?w=739" alt="" width="739" height="189" />
