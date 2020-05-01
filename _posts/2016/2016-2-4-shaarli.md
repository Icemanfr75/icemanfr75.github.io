---
layout: post
title: Tutoriel - Créer son flux RSS...même sur mobile
category: tuto
tags: android, RSS, shaarli, tutoriel, wordpress
---
**J'en avais parlé à la création de cette version du blog. On peut assez facilement créer un fil RSS regroupant une sélection d'articles ou sites intéressant. Afin d'être cohérent avec le logiciel libre, je me suis orienté vers l'utilisation de Shaarli, pour sa facilité d'installation.**

Créé par Sebsauvage, ce petit programme s'installe même sur une simple page perso free, à condition de créer un répertoire "Session" et d'intégrer un fichier nommé ".htaccess" (attention au . devant) et qui comprendra le texte suivant :

<blockquote>
<pre class="code">php 1
SetEnv PHP_VER 5</pre>
</blockquote>

Mais Seb explique cela très bien sur son site : <a href="http://sebsauvage.net/wiki/doku.php?id=php:shaarli#installation">http://sebsauvage.net/wiki/doku.php?id=php:shaarli#installation</a>

Ce qui est moins dit, c'est la possibilité d'utiliser cet outil sur son mobile Android. Sur un navigateur classique, on peut installer un raccourci pour partager une page dans son flux RSS. Mais sur mobile, c'est moins évident, à moins d'utiliser l'appli baptisée fort intelligement <a href="https://play.google.com/store/apps/details?id=com.manatlan.tools.share"><span style="text-decoration:underline;">Shaarli</span></a>. Après avoir lancé une première fois cette application un peu bricolée, on entre l'adresse de son Shaarli personnel. Ensuite, le choix "Shaarli" apparaitra dans le choix de partage d'Android.  Bon, il faut avouer que la fenêtre est parfois un peu grande pour un mobile trop petit mais ça fonctionne suffisamment pour alimenter son flux RSS à tout moment de la journée.

En ce qui concerne l'intégration à son site wordpress, il suffit d'aller dans les Widgets (menu Apparence) et d'entrer l'adresse du RSS de son Shaarli (dans le menu en haut de l'interface Shaarli) dans ce widget au doux nom de RSS. Et voilà le travail. Simple, non ?
