---
layout: post
title: Tuto - 2 petites astuces Flickr pour avoir des flux RSS
category: tuto
tags: flickr, flux rss, geek, RSS, tutoriel
---
**Vous utilisez peut-être ce service de partage de photo et de stockage qu'est Flickr. Voici deux petites astuces pour avoir du <a href="https://fr.wikipedia.org/wiki/RSS">flux RSS</a> dedans**

Tout d'abord, il est utile d'avoir son ID Flickr, un truc en #######@N## à la place de son identifiant habituel. Il peut s'obtenir simplement avec cet outil : <a href="https://www.webpagefx.com/tools/idgettr/">https://www.webpagefx.com/tools/idgettr/</a>

**Comment connaître l'adresse de son flux RSS ?**

rajoutez tout simplement ?details=1 à l'adresse de votre galerie et tout en bas, vous allez voir apparaître une icone orange de flux RSS.

<img class="aligncenter wp-image-22990 size-full" src="https://cheziceman.files.wordpress.com/2018/05/fluxrssflickr.jpg" alt="" width="362" height="44" />

Un clic droit sur l'icone vous donnera l'adresse du flux à inclure. Oh surprise, vous devez retrouver votre ID Flickr dedans :

https://api.flickr.com/services/feeds/photos_public.gne?id=**<span style="color:#ff0000;">IDFLICKR**&amp;lang=fr-fr&amp;format=rss_200

Pour le mien, ça donnera par exemple, https://api.flickr.com/services/feeds/photos_public.gne?id=76217081@N04&amp;lang=fr-fr&amp;format=rss_200

Pour info pour les utilisateurs de #flickr, vous pouvez obtenir le flux ATOM/RSS de vos favoris avec une adresse du type :

https://www.flickr.com/services/feeds/photos_faves.gne?id=<span style="color:#ff0000;">**IDFLICKR**&amp;lang=en-us&amp;format=atom

Le format peut être changé en ATOM comme vous pouvez le voir dans la balise format, ci dessus. Je vous laisse deviner maintenant quelles photos je sélectionne...
