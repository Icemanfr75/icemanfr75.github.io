---
layout: post
title: Blog - Doit-on vraiment héberger son site wordpress ?
category: geek, tuto
tags: auto hébergement, blog, geek, Geekeries, Réflexion, web, webmastering, wordpress
---
**Derrière cette question, il y a la propriété de ses écrits. Est-ce que tout ce que vous trouverez ici est ma propriété ou celle de la société propriétaire de Wordpress.com ? Le Creative Commons n'aurait pas une grande force si demain on s'emparait de cela...**

C'est un peu pour cela que j'ai remis en place un blog Wordpress à son <a href="http://iceblog.free.fr">emplacement initial</a> et qui me sert de "backup". Cela m'a permis de peser le pour et le contre des deux solutions, selon le temps que l'on veut passer à tout cela. Cet article est un peu l'équivalent de celui lu sur <a href="https://www.crazyegg.com/blog/reasons-to-use-wordpress/">Crazyegg,</a> mais n'est absolument pas une traduction.

**Personnaliser, adapter...**

Après avoir pas mal travaillé sur la personnalisation sur les anciennes versions (voir Joyeux Végé) quand il manquait beaucoup de choses, maintenant, on trouve l'essentiel sur les versions standards, qu'elles soient Wordpress.com ou hébergées. Ainsi, je suis parti ici d'un thème et j'ai rajouté quelques petits éléments distinctifs. Il y en a énormément aujourd'hui, même si je trouve qu'on devrait faire le ménage dans les versions qui ne sont plus "responsive". Coté hébergement, Free me limite beaucoup et c'est plutôt lent donc j'ai cherché la simplicité. Ailleurs, je n'aurais pas ce problème. Mais un blog reste un blog, donc l'essentiel est dans le texte, voir les images si on est plus dans le dessin et la photo. Pas besoin d'en faire trop coté personnalisation. Surtout que ça peut poser des problèmes dans les mises à jour. Car si on se base sur un thème qui n'est plus développé ensuite, pour les prochaines versions de Wordpress, catastrophe en perspective. Toute modification sur un thème doit être écrite quelque part pour reprendre éventuellement cela sur un autre thème.

**La Sécurité**

Avoir un blog hébergé, ça veut dire qu'on va faire les mises à jour de sécurité soi-même, modifier son fichier htaccess, sauvegarder ses billets, etc... Si on n'aime pas ça, c'est sur que Wordpress.com garantit un haut niveau de service avec de la sécurité et tout ça sans payer...enfin si, on se tape des bandeaux de publicité en échange. Bien sûr, tout ça ne paraît pas sorcier, finalement et je n'ai pas eu de blogs piraté jusqu'ici. Il faut dire que j'utilise peu de plugins, le nid à emmerdes. Mais la dernière faille de wordpress, non corrigée depuis un paquet de temps, peut inquiéter.

**L'intégration de médias**

C'est en exportant ce blog que je me suis aperçu d'un petit détail qui a son importance. Wordpress.com intègre Jetpack, un gros plugin qui fait beaucoup trop à mon goût, dont des stats....et qui ne passe pas chez Free. Donc ce qu'on appelle le shortcode youtube ne passe plus. Il s'agit d'un moyen simple d'intégrer des vidéos youtube (ou autres) en tapant [la video](adressedelavideo ... ] au lieu d'aller chercher le code en &lt;iframe ....&gt; Quand on exporte, c'est tout à refaire. Bof, ce n'est pas grave donc je laisse comme ça, idem pour les liens bandcamp, soundcloud que j'avais mis. Autre souci, la bibliothèque de média est exportable à travers un XML... mais seulement si l'hébergeur admet d'intégrer automatiquement des sources externes. Ce n'est pas le cas de Free mais ça marchera ailleurs. Il existe de multiples plugins pour des intégrations de médias mais il faut penser que l'on devient dépendant du plugin si on déménage le blog. Donc comme d'habitude, moins de plugins, c'est aussi moins d'emmerdes plus tard. Il y en a quand même des utiles.

**Le coût**

Quand on débute, évidemment, on se dit qu'on va d'abord essayer et si ça nous plaît, on paiera peut-être. J'en connais beaucoup qui ne tiennent que 3 à 6 mois, après avoir épuisé toutes leurs idées. J'ai moi même des creux d'inspiration (je triche pour que ça ne se voit pas, grace à la planification...). De ce coté là, Wordpress.com reste le tremplin idéal qui permet de découvrir le produit sans s'emmerder. Un ancien chroniqueur d'Histozic a ainsi sauté le pas avec un succès relatif et j'en connais d'autres à qui j'ai mis le pied à l'étrier. Free et les hébergeurs gratuits proposent des solutions intermédiaires mais limités techniquement. On peut tout de même s'en sortir sans trop de soucis par des associations et des hébergeurs sans aller jusqu'au nom de domaine. L'avantage de Wordpress reste dans ses nombreuses possibilités d'import et d'export, ce qui fait qu'on peut pratiquement tout déplacer sans trop de souci en suivant des règles simples. Les autres CMS n'ont évidemment pas l'histoire et les capacités de développement du géant US.

**Conclusion**

J'ai fait un choix qui n'a rien de définitif et j'ai tout essayé (nom de domaine, hébergé payant, gratuit, wordpress) à différents moments de la vie. C'est en effet comme ça que ça marche. La vie nous change et il n'y a aucune solution meilleure que les autres, sinon de savoir ce à quoi on s'attend. Avec l'age, on a envie de faire simple, de moins expérimenter et wordpress.com me suffit finalement bien. Comme je suis un peu paranoïaque, j'ai ma solution de secours, au cas où Wordpress se ferait racheter par un dangereux milliardaire nord-coréen (en ce moment, c'est eux les méchants...) qui déciderait que tout lui appartient. Il est noté partout que ça m'appartient mais bon, ce n'est pas non plus la fin du monde si ça disparaît. Ceinture et bretelle, c'est toujours mieux et ce qui est valable pour ses données personnelles l'est aussi pour son blog : PENSEZ A SAUVEGARDER. Je ne dis pas de le faire tous les jours, mais par trimestre, ou semestre, c'est pas mal. Et la clé, c'est le temps qu'on veut passer à ça, avec derrière la volonté d'apprendre des choses ou pas.

Pour résumer :

 * 1) Tu n'as pas le temps, tu veux rester dans ton ignorance crasse : Tu fais rien !
 * 2) T'as un peu de temps et tu veux (éventuellement) bricoler un peu ton site : Wordpress.com
 * 3) T'as du temps et tu veux apprendre des choses sur l'hébergement : Hébergeur de ton FAI ou un hébergeur de taille moyenne/association
 * 4) T'as vraiment le temps de t'intéresser à ça et tu veux apprendre : Autohébergement ou gros hébergeur qui t'enverra chier quand tu l'appelle.

Un double du site en local pour se faire la main, c'est aussi pas mal...sur les cas 3 et 4. Et ça sera la folie dans la maison !

[la video](https://www.youtube.com/watch?v=rXuvdeEC5y8)

