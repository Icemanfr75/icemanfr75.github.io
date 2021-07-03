---
layout: post
title: Tuto - Dompter Firefox Android, ou pas ? 
category: tuto, 
tags:  tutoriel, mobile, web
---

**Je suis repassé sur Firefox sur mon mobile (après y être revenu sur mon PC qui n'est plus limité en mémoire), malgré quelques bémols (personne n'est parfait) mais en me penchant sur la configuration du navigateur. Car par défaut, ce n'est pas suffisant et pas toujours très clair.**

### Présentation

**Pourquoi Firefox ?** Parce que c'est le dernier moteur de rendu Web réellement alternatif, tout le reste étant plus ou moins dans la nébuleuse Google Chrome. Oui Opera, c'est aussi un dérivé, donc Vivaldi. Et Brave aussi, même si on retire tout ce qui est Google, c'est bien le géant américain qui dicte les standards du web. Alors même si la gouvernance de la fondation Mozilla est parfois n'importe quoi, je continue de soutenir le moteur de Firefox.

Pour **Firefox sur Android**, vous avez le choix entre la version normale (celle que j'utilise ici), la Beta qui est un produit déjà beaucoup testé mais non exempt de bugs potentiels, et la Nightly qui est la version de développement la plus en pointe et qui sert de test grandeur réel. A réserver à un public averti pour cette dernière. La version normale a donc un look un peu différent d'autres navigateurs avec sa barre d'adresse en bas et ... l'absence de Speed Dial pour d'autres solutions plutôt alambiquées. Ah oui, il y a encore Firefox Focus qui n'a  pas de gestion de favoris et est donc une solution bien limitée qui disperse un peu plus les forces. 

On a accès aussi à des **plugins/extensions** mais de manière très limitée, ou ciblée. On retrouve les µBlock Origin, Ghostery, Privacy Badger, HTTPS Everywhere...et même Bitwarden même si je ne vois pas l'intérêt par rapport à l'application qui elle fonctionnera sur tous les produits du téléphone. On verra que ce n'est pas sans contrepartie. Il y a aussi un mode lecture qui peut faciliter la chose sur quelques sites. On retrouve la possibilité de mettre en thème sombre l'interface, parce que forcer les sites ne fonctionne pas vraiment. Les onglets peuvent se gérer par mosaïque ou liste avec l’aperçu. 

*Pour mémoire, j'utilise un Xiaomi Redmi4A avec son Snapdragon 425 et seulement 2GO de RAM. Cela explique quelques résultats et donc mon choix final.*

![image](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2021/firefox1.jpg)

*Le premier réglage à faire, c'est de mettre la confidentialité à jour...strict, ça fonctionne pas mal*


### Utilisation

Ce que j'ai commencé par faire par habitude, c'est de mettre µBlock Origin et là, j'ai vu que ça ralentissait beaucoup trop. Pour comparer, j'ai enlevé µBlock et mis la protection native de Firefox au "max". J'ai trouvé que cela fonctionnait bien mieux mais il faut dire que j'utilise aussi [Blokada](https://blokada.org) en tâche de fond, ce qui supprime aussi beaucoup de publicités et autres malveillances commerciales ou espionnes. Je déconseille donc de rajouter des plugins si on est un peu juste en mémoire et CPU sur son mobile. 
 
Niveau **utilisation mémoire**, on est à 20% en moyenne au dessus d'Opera ce qui reste très correcte, ou similaire à d'autres navigateurs premium du marché. Je n'ai pas remarqué de saturation mémoire façon Firefox Desktop mais parfois des ralentissements inexpliqués que je ne rencontre pas sur Opera mais que j'avais aussi sur Chrome. Je pense là aussi que l'utilisation mémoire est en cause. 

Pour tous les jours, je trouve que l'alliance avec Bitwarden est un peu plus fluide qu'avec Opera. La barre d'adresse en bas est une bonne idée mais il y a quelques petits bugs de chevauchement avec le clavier. Le mode privé est très accessible et fonctionne bien. 

Par contre, je n'ai rien compris dans la **gestion des marque-pages** qui sont dans des bibliothèques ou pas, dans des tiroirs. La synchronisation fonctionnerait bien mais pourquoi mettre les marque-pages mobiles à part, ne pas pouvoir en afficher certains en page d'accueil et les gérer ainsi alors que là c'est une gestion séparée ou impossible. On peut créer des catégories/collections mais ce ne sont pas non plus des marque-pages, plutôt des raccourcis internes. Sur les trois possibilités , tous ne se synchronisent pas. A un moment, il faut choisir et tant qu'à vouloir se singulariser, autant le faire dans l'intérêt de l'utilisateur. Là c'est l'inverse. 

![image](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2021/firefox6.jpg)

*Exemple de la mauvaise idée des collections par rapport aux raccourcis et marque-pages*

Il n'y a pas de **bouton de sortie** pour fermer correctement. Je sais que cela paraît peu important mais quand on est juste en mémoire, cela prend du sens. Il y a une solution : Il faut dire que l'on ne veut pas conserver des données dans les paramètres et dans ce cas, un bouton quitter apparaît dans le menu. J'ai par exemple fait le choix de vider le cache à chaque fois et c'est vraiment très bien, mieux que sur Opera qui est en tout ou rien. 

![image](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2021/firefox2.jpg)

*Aller dans le menu des paramètres pour modifier "supprimer les données en quittant*

![image](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2021/firefox3.jpg)

*A minima, je conseille ça. On peut aussi supprimer les cookies, l'historique...*

![image](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2021/firefox4.jpg)

*Dans le paramètre "Collecte des données", libre à vous de participer à l'amélioration, comme pour la Nightly*

Un des plus de Firefox c'est de choisir son moteur de recherche par défaut car beaucoup d'autres navigateurs sont limités. DuckDuckgo pour ma part.

![image](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2021/firefox5.jpg)

Si certains sites avec leurs pop-ups RGPD fonctionnent mieux sur Firefox Android que Opera, j'ai des **"Force Close"** reproductibles comme j'en ai souvent eu avec Firefox Desktop, ce que je n'ai pas au même endroit avec les concurrents. C'est aussi pour ça que je conseille toujours d'avoir deux navigateurs sur une machine pour parer aux blocages de ce type. C'est quand même de l'ordre du 0,1% des sites donc peu dérangeant. 

### Ce qu'il manque

* Les **pages hors-connexion** façon Opera sont un plus bien pratiques que je n'ai pas retrouvé, même si on peut exporter une page ici. 
* Le [Speed Dial](https://en.wikipedia.org/wiki/Features_of_the_Opera_web_browser#Speed_Dial), qui pour moi est devenu un standard. Même en version Desktop c'est devenu n'importe quoi entre les conseillés, les éléments clés, les sites visités et donc les collections ou bibliothèques dans lesquelles sont ...
* ...les **Marque-pages** : Avoir une gestion simple et unique sur tous les produits firefox. 
* L'intégration d'un **VPN**...Bon Firefox s'y met en mode payant mais l'intégration directe dans le navigateur android comme Opera est un vrai plus (à noter qu'Opera Desktop ne le met qu'en plugin). J'imagine que cela arrivera, il faut que je mette la Nightly à nouveau. 
* Un **plug-in Gemini**, Gopher ? Bon franchement, c'est pour faire plaisir à tous les geek qui se mettent en tête de revenir au basique. 
* Les **Containers**, ce plugin plutôt intéressant pour isoler les données de certains sites espions par rapport au reste. Mais je crois que c'est déjà dépassé...

### Bilan

J'ai passé un mois sur ce navigateur sur mon mobile et ... je suis revenu à mon fidèle Opera par défaut (depuis 3 ans) qui globalement réunit ce que je veux avec le petit plus du VPN quand j'en ai besoin, malgré ses performances limitées. Firefox n'est plus très loin de ce qu'il faudrait mais j'ai eu de nombreux force-close et des ralentissements par rapport à son concurrent. Attention, elles sont au niveau d'un Chrome sur le même terminal, l'ergonomie du navigateur de Google n'étant pas exemptes de critiques. 

Bref, dans mon petit classement personnel, je mets toujours Opera en premier mais mon second choix est de loin Firefox. Je pense que sur des terminaux plus récents avec plus de mémoire, ça le fait très bien. J'ai juste peur que l'on ne disperse encore les efforts de développement sur des voies sans issues, entre le Firefox Focus qui ne devrait être qu'une option (car en navigateur léger on trouve mieux aussi), le VPN et d'autres lubies ergonomiques inutiles.


Bande son : [Gary Moore reprenant le Foxy Lady de Jimi Hendrix ![video](/images/youtube.png)](https://www.youtube.com/watch?v=LjUZ0amX4EI){:target="_blank"}
