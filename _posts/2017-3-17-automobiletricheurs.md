---
layout: post
title: Automobile - Alors, tous tricheurs, les constructeurs?
category: automobile
tags: Automobile, cartographie, dieselgate, pollution, psa, renault, tricherie, volkswagen
---
**On a l'impression, avec le <a href="https://cheziceman.wordpress.com/2015/10/03/automobile-comment-ne-plus-revivre-laffaire-volkswagen/">Volkswagengate,</a> le Renaultgate, le <a href="http://money.cnn.com/2016/04/26/news/companies/mitsubishi-cheating-fuel-tests-25-years/">Mitsubishigate,</a> etc que tous les constructeurs automobiles sont des tricheurs. Comme si en Politique, on disait tous pourris ?**

Bon, pour prouver le contraire ou pas, je vais devoir expliquer un peu le truc. Déjà, il faut rappeler qu'il existe des <a href="https://cheziceman.wordpress.com/2015/05/08/automobile-la-consommation-de-carburant-et-ses-secrets/">normes de cycles</a> pour mesurer consommation et pollution et qui ont l'avantage d'être répétables, mais l'inconvénient d'être peu réalistes, notamment par des accélérations trop lentes. Forcément, les constructeurs se sont entendus pour ça... Même la norme qui sera appliquée prochainement est trop conciliante, mais plus longue en temps/distance. Des petits malins (chez les équipementiers ...puis les constructeurs) ont trouvé le moyen de détecter ces cycles et d'optimiser les moteurs pour cela, ... mais pas pour le reste du fonctionnement. Enfin, là, je caricature.

Il faut que j'explique le terme "**Cartographie moteur**". Non, ça n'a rien à voir avec le GPS. Depuis que les moteurs embarquent des injections électroniques et des calculateurs, on peut agir sur le comportement du moteur. En compétition, on va le faire avec comme objectif une réponse optimale à ce que demande le pilote par son action sur la pédale, avec des valeurs de couple, de puissance et en évitant trop d'à-coup, par exemple. Mais dans la vie de tous les jours, ce n'est pas la performance qui sera recherchée mais un mélange entre le confort, la consommation, les émissions. Et là, il y a des choix à faire. Cette cartographie consiste donc en un ensemble de réponses à des paramètres, comme l'appui sur la pédale, le régime du moteur, la température, la pression, etc...On parle de cartographie car si on représente ces courbes, ça ressemble un peu à des paysages et surtout ça localise le point de fonctionnement où se situe le moteur. Par exemple, je pique à l'université de Lausanne pour la consommation :

<img class="wp-image-9189 aligncenter" src="https://cheziceman.files.wordpress.com/2017/03/cartoconso.jpg?w=300" alt="" width="481" height="337">

Un peu comme si pour cuire le rôti au goût de tout le monde, vous aviez des capteurs de température dans et autour du rôti pour commander le thermostat du four à tout moment. Les paramètres sont nombreux et la mise au point d'un moteur consiste à créer la meilleure cartographie pour répondre à un cahier des charges. Dans ce cahier des charges, il y aura d'abord les normes antipollution, la consommation, mais aussi l'agrément client ce qui se traduit en vibrations, en bruit, et aussi la fiabilité, sans parler de la puissance et du couple moteur. Petit souci, antipollution et consommation sont parfois deux intérêts opposés dans les réactions chimiques et thermodynamiques qui se font dans le moteur (voir schéma ci dessous). Ainsi, on peut diminuer de la consommation, donc du CO2, mais créer trop de NOx ou de particules. **Tout est affaire de compromis**. Ce compromis sera fait par rapport à des profils d'utilisation.... ça va, je ne vous ai pas encore perdu, là? Tiens, un petit parallèle avec l'informatique : Une carto ça s'upload comme un firmware, si on a le bon soft pour y accéder. Et il y a des boites qui vous vendent des cartographies/calculateurs reprogrammés pour avoir plus de puissance, mais à quel prix ? Nul ne le sait vraiment car à part des essais perfo sur banc, il n'y a pas assez de retour en fiabilité.

<img src="http://www.endtuning.com/images/airfuel.jpg" alt="" width="376" height="354">
ici, on voit un exemple d'émissions avec les zones où le moteur consomme le moins, où il est le plus puissant, etc...

Oui, le moteur d'une voiture ne va pas répondre pareil en ville ou sur autoroute à un régime bien stabilisé. Il ne répondra pas pareil si le conducteur appuie très vite sur la pédale ou s'il est très doux. Et il ne répondra pas pareil avec le fameux cycle ou un démarrage à froid à Stockholm un 25 Février, ou à La Paz un 15 Aout. J'ai vu des cas de&nbsp;problèmes de démarrage en côte,dans la cordillère des Andes&nbsp;qu'il faut résoudre et en même temps répondre à des problèmes opposés, comme les bouchons des villes sud-américaines. Donc il est possible de bien faire son boulot pour répondre à la norme, sans système de détection, mais d'avoir totalement foiré une carto sur un environnement d'essai différent, voir rare. C'est le but des bancs d'essais moteurs et des campagnes d'essais réelles, en mission chaudes, froides. Mais tout ça coute de l'argent et il y a la pression des jalons du projet pour **sortir le véhicule à temps.** Dans cette histoire de compromis, on vise très souvent la réponse à la norme de test, la conso par rapport à la concurrence et l'agrément de conduite, puis le reste un peu plus tard. J'ajoute que le constructeur a aussi d'autres paramètres à faire varier, comme par exemple les rapports de boite de vitesse.

Aujourd'hui, **avec les tests en réel** comme ce qui arrive maintenant avec les <a href="https://cheziceman.wordpress.com/2016/04/12/automobile-le-dieselgate-devoile-un-autre-piege/">PEMS</a> (je rappelle qu'il s'agit de systèmes de mesure embarqués dans une voiture), et les normes plus sévères sur les NOx, les constructeurs sont bien embêtés. Pour les NOx, j'avais parlé des deux technologies proposées et du fait que la technologie NOxTrap était moins performante mais moins coûteuse. Pas de chance, c'est celle que Renault a choisie et dans les échanges de mails visés par l'enquête, il peut y avoir interprétation. Je pense que Renault était tout à fait conscient que son système répondait à la norme mais ne marchait pas du tout dans certaines conditions, car tous les constructeurs ont testés les différentes solutions des équipementiers (Delphi, Bosch, Continental, Valeo, etc...) avant de valider un choix. Pour les véhicules incriminés chez Renault, ça représente un gain total d'environ 1,5 milliards, voir 2 milliards sur cette période de production. Le fait de détecter ou pas le cycle, est très secondaire à ce moment du choix. Mais on peut reprocher, tout comme à l'équipementier, cette solution de rustinage. Même la technologie SCR concurrente, choisie par exemple par PSA, n'est pas exempte de reproches et une cartographie aura des "trous". C'est sans doute ce qui a été repéré par l'organisme italien sur le C4 Cactus, encore que...

<img class="size-medium wp-image-9193" src="https://cheziceman.files.wordpress.com/2017/03/cartologiciel.jpg?w=300" alt="" width="300" height="157">
une carto tout prête à être intégrée

Il faut **rétablir quelques vérités** par rapport à ce que les journaux ont présenté. Il n'y a pas dépassement des émissions de CO2 de 300% chez Renault. Ce sont les émissions de NOx, sinon nous aurions des consommations tellement&nbsp;élevées que les conducteurs iraient rendre leur voiture. Mais pour les NOx, les fabricants des systèmes de mesure embarqués ne savent pas aujourd'hui garantir des mesures représentatives et répétables, malgré les dires des commerciaux dans les instances européennes. Ce n'est pas le type de capteur ou l'étalonnage qui est en cause mais les algorithmes servant à "recaler" les mesures dans des conditions comparables aux bancs et proposer des valeurs pour les types d'utilisation. Les matériels sont encore en phase de validation, en Allemagne, Japon, Etats-unis. Disons qu'à minima, il y a des tendances mais pas de certitudes sur les valeurs absolues. Enfin, les futures procédures d'essais en conditions réelles sont toujours en discussion sur des points de détail, de même que les mesures de consommation électrique pour les véhicules hybrides et rechargeables, où là aussi on est dans le flou le plus complet pour le consommateur.

**Peut-on dire que tout le monde a triché?** Oui et non. Tout le monde répond à une norme à sa manière et essaye de cibler des conducteurs type dans des conditions type pour tirer le meilleur rendement. Une consommation trop importante et un mauvais agrément seront sanctionnés par le consommateur, mais pas une pollution trop importante et c'est là le souci. Le consommateur n'a pas idée de sa pollution due par exemple à une mauvaise utilisation, voir un mauvais entretien (les nouveaux systèmes sont sensibles). Il n'y a pas des capteurs dans la voiture qui donnent ce qu'on envoie comme saloperies dans l'air. On n'a pas assez dit qu'un diesel ne sait pas fonctionner à froid en ville, ou que l'hybridation est conçue pour combler les manques des moteurs thermiques, plus ou moins bien. Donc les constructeurs n'ont pas tous triché mais ont tous &nbsp;masqué certaines parties peu reluisantes de leurs cartographie qu'ils espèrent rares en fonctionnement réel. On a même "d'heureuses" surprises sur des véhicules plus polluants dans les normes que d'autres, et qui s'avèrent pas si mauvais en conditions réelles. Au moins, avec les normes à venir et les <a href="http://media.groupe-psa.com/fr/communiqués-de-presse/groupe/le-groupe-psa-publie-consos-usage-reel">modélisations,</a> saura-t-on mieux choisir ce qui convient à chaque typologie d'utilisation. Mais arrêtons une bonne fois pour toute de parler de véhicules "propre", car par définition, ça n'existera jamais, même si on y mettait tout l'or du monde.
