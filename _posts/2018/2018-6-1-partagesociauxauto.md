---
layout: post
title: Tuto - Comment diffuser sur tous les réseaux sociaux sans se fatiguer ?
category: tuto
tags: diaspora, facebook, flux rss, information, mastodon, réseaux sociaux, tutoriel, twitter
---
**Pour ceux qui aiment être un peu partout mais ne veulent pas y passer trop de temps, ni d'argent (parce qu'il y a des outils commerciaux pour ça), il est possible de pratiquer les réseaux "libres" ou non de manière automatisée ou semi automatisée. Je parle donc ici de Diaspora, de Mastodon mais aussi de Twitter et ça peut être étendu à Google Plus, Facebook pour ceux que ça intéresse, à leurs risques et périls.**

L'idée est d'avoir, par exemple, la diffusion d'un nouveau post sur ce blog sur chacun des réseaux sans la moindre intervention. Je n'utilise pas la fonction "Publicize" de Wordpress qui se contente des gros réseaux. Je n'utilise pas non plus de plugins qui ne sont pas installables sur Wordpress.com en version gratuite.

Pour ceux qui utilisent encore Diaspora* (ça devient rare ), on va devoir lier Diaspora et Twitter, sur une instance qui dispose de cette fonction (vérifiez mais c'est normalement assez courant sur les grosses instances sérieuses). C'est dans "/services" dans votre instance préféré qu'il faut aller. L'enchaînement idéal est **Diaspora-Twitter-Mastodon**. Mais Twitter peut aussi s'interfacer avec d'autres réseaux que Mastodon. Lorsque vous créez un post sous Diaspora* il faut mettre en surbrillance le petit &lt;t&gt; bleu sur la gauche de la fenêtre de saisie ou bien le petit oiseau, selon la version. Ainsi il sera dupliqué sur votre profil Twitter.

<img class="aligncenter size-full wp-image-22877" src="https://cheziceman.files.wordpress.com/2018/04/diaspotweet.png" alt="" width="590" height="241">

Pour ce qui est d'**envoyer un billet de blog Wordpress** sur votre instance de Diaspora*, j'ai déjà <a href="https://cheziceman.wordpress.com/2016/01/12/tutoriel-ajouter-un-bouton-de-partage-diaspora-a-son-blog-wordpress-com/">pratiqué ici</a>. Mais pour ceux qui n'utilisent plus Diaspora*, alors il reste à mettre la fonction publicize de Wordpress en route ou bien d'utiliser<a href="https://ifttt.com/discover"> IFTTT</a> pour automatiser la tache Wordpress vers Twitter et compagnie. Je préfère cette dernière solution qui évite d'avoir à recopier à chaque fois une petite explication du billet de blog en introduction, si ce n'étaient des petits soucis avec les tags. Il s'agit de définir une condition SI (IF THIS) et ensuite d'en définir une conséquence (THEN THAT). Par exemple vous pouvez dire que s'il y a un nouveau post sur votre fil Twitter, ça créera un post sur votre fil Facebook, Google+, Linked In. L'avantage est de ne pas avoir à aller sur ces multiples réseaux tout en étant présent. Le problème est que ça ne marche pas avec Mastodon et ses différentes instances. Il y a bien une méthode en créant une "application" personnelle pour Mastodon mais j'ai trouvé plus simple (mais aussi plus risqué?)

Il suffit d'aller dans l'outil<a href="https://crossposter.masto.donte.com.br/">&nbsp;https://crossposter.masto.donte.com.br/ </a>qui permet d'assurer la transition entre Mastodon et Twitter. Il faut au préalable se connecter sur les deux réseaux sociaux puis aller dans les options pour mettre sur ON la réplication des tweets sur Mastodon (l'inverse est évidemment possible). Vous pouvez aussi le faire dans les deux sens, définir les actions pour les réponses, les retweets, etc. Mais l'absence de bookmarklet et/ou de bouton universel pour Mastodon montre le faible avenir de ce réseau auprès du grand public.

On a donc déjà l'automatisation Diaspora* jusqu'à Mastodon mais Wordpress alors? Il y a bien des projets github qui automatisent du RSS sur Diaspora mais l'intégration n'est pas aisée/possible pour un simple utilisateur. J'ai aussi un bouton Diaspora sur le blog&nbsp; afin de pouvoir partager simplement du contenu. Mais j'en suis venu à me demander l'utilité du partage sur un réseau qui a tendance à mourir. Au pire, il y a l'intégration d'un plugin si vous avez un wordpress autohébergé. Je préfère faire encore à la main sur une sélection d'article.

Et puis en bonus, il y a la possibilité de diffuser automatiquement les articles préférés de votre flux RSS. J'utilise pour cela <a href="https://theoldreader.com/">TheOldReader,</a> mais ça marcherait aussi si vous utilisez <a href="https://github.com/sebsauvage/Shaarli">Shaarli</a>. Ma sélection d'article se retrouve dans son propre flux RSS correspondant à mon profil (ici c'est&nbsp;<a href="https://theoldreader.com/profile/iceman75.rss">https://theoldreader.com/profile/iceman75.rss</a> ). J'ai donc créé une "applet" IFTTT qui va recopier tout nouveau post de ce flux RSS (le This) pour en faire un nouveau Tweet (le Then). Et comme derrière les Tweets deviennent des posts de Mastodon, je n'ai rien d'autre à faire que "partager" dans mon fil RSS. Inutile donc, pour moi, d'aller dans Twitter ou Mastodon et compagnie, tout en partageant de l'information. Après, c'est sur que ça n'aide pas au dialogue qu'il peut y avoir après. Mais le vrai dialogue ne doit-il pas se faire sur les articles et pas dans les réseaux sociaux? Ou même sur un forum...