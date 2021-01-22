---
layout: post
title: Tuto mobile - Bloquer les publicités sur son smartphone android
category: tuto
tags: android, geek, Geekeries, mobile, publicité, tutoriel, Tutoriels, vpn
---
**Si la plupart des utilisateurs de smartphones ont un bloqueur de publicité dans le navigateur (plus ou moins efficace), il reste des publicités dans les applications ainsi que des "fuites" potentielles vers Google et le constructeur du smartphone. Difficile de tout bloquer mais au moins peut-on limiter les dégats... sans être<a href="https://fr.wikipedia.org/wiki/Utilisateur_root"> root</a>.**

L'astuce consiste à passer par la fonction VPN d'Android et j'étais un peu sceptique, sinon inquiet de ce qui pourrait se passer. J'ai testé DNS66 mais sans trouver cela très efficace. Je lui ai préféré le récent <a href="https://blokada.org">Blockada</a>, qui est opensource, avec une interface plus glamour même s'il vaut mieux parler anglais. Vous ne trouverez aucun de ces programmes dans le playstore puisque justement ça va contre les intérêts de Google et ses publicités ciblées. Profitons-en... Il faut donc toujours télécharger <a href="https://github.com/blokadaorg/blokada/releases/download/4.1.6/blokada-v4.1.6.apk">l'APK</a> puis faire installer après avoir autorisé les applications tierces, ce que vous devez savoir faire si vous avez suivi mes précédents tutos (sinon Qwant/Duck Duck Go est ton ami pour trouver comment faire sur votre version d'Android). 

Si j'étais sceptique sur le principe du vpn c'est qu'on a vu des abus par des VPN gratuits qui récupèrent ni vu ni connu les données utilisateurs en passant. Le fait d'avoir un programme open source, d'être passé entre les fourches caudines de nombreux forums spécialisés permet d'avoir une certaine confiance dans ce produit qui en est à la version 4. J'ai regardé aussi quelques logs de connexion pour voir ce qui se passait lors de l'utilisation et testé sur applications et sites pour voir le résultat. Ca marche mais il convient de savoir utiliser correctement le produit. 

![image](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2019/blockada_demar1.png)

*Dans la liste des autorisations de démarrage*

![image](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2019/blockada_demar2.png)

![image](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2019/blockada_permis1.png)

*Dans les paramètres de l'application dans Android*

![image](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2019/blockada_permis2.png)

*Dans les paramètres Android de l'application, rubrique autres autorisation*

**Le garder en tache de fond** : Si comme moi vous avez une rom Android configurée pour tuer les applications qui ne servent pas et en empêcher de démarrer toutes seules, alors Blockada ne va pas aimer. Il faut donc commencer par lui céder des droits élémentaires. Vous verrez apparaître alors une notification VPN dans le haut de l'écran lorsqu'il fonctionne. Malheureusement, lors de l'utilisation de gros jeux gourmands en RAM, il peut arriver que la ROM ferme tout ce qui dérange et il faudra forcer ou attendre le redémarrage de Blockada dans ce cas. Je conseille de garder les notifications pour voir ce qui est bloqué... si une application/site refuse de fonctionner, ça aide à comprendre. 

![image](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2019/blockada_main.jpg)

*Il y a juste ça à lancer (ça se met en vert)*

Voici les écrans de configuration de Blockada à minima, c'est à dire avec non pas la fonction de vrai VPN mais uniquement le filtrage de données entrantes et sortantes. Pour vous faire peur, dites vous bien que j'ai eu 50000 blocages en 1 semaine, c'est dire si on vous en veut... ou plutôt on en veut à vos données. Ainsi j'ai vu qu'Opera envoyait des données de personnalisation, que Flickr continuait à aller chez Yahoo, que Firefox ne fait rien mais que les sites veulent envoyer des données chez les analytics de toutes sortes, que FFBE a pas mal d'appels à des sites que l'on peut bloquer sans perturber le fonctionnement du jeu. On peut aussi mettre une application en liste blanche c'est à dire lui laisser tout faire... à vos risques et périls. 

![image](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2019/blockada_blacklist.png)

*Une liste noire pour commencer, c'est bien*

Je préfère aller voir dans la liste du journal ce qui se passe pour faire un peu d'apprentissage et bloquer moi même ce qui me dérange. Si vous utilisez le Google Play store ou Waze, il faudra les laisser faire beaucoup de choses, malheureusement. 

![image](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2019/blockada_journal2.png)

*C'est là que l'on voit ce qui se passe et qu'on peut bloquer certains accès...*

![image](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2019/blockada_journal.png)

*Par exemple là, on voit que Facebook rode... mais attention si vous en avez besoin pour accéder à la page de ce réseau ou si un jeu utilise ce compte ?*

![image](https://filedn.eu/llqi9IBxlYouGRXYG2xlROb/img/2019/blockada_blocked.png)

*Et là on voit les domaines bloqués !*

Voilà déjà pour assurer vos premiers pas avec cette application. Si un blocage gène une application, vous avez le choix de remettre l'autorisation de ce site ou bien de tout permettre à l'application. Je préfère faire site par site mais c'est plus long. A vous de voir et de faire vos retours... voir d'autres solutions avec des listes personnelles. 

Je termine par une vidéo de présentation en anglais (avec accent) qui permet de voir l'ensemble des possibilités du programme.

En video : [![video](/images/youtube.png)](https://www.youtube.com/watch?time_continue=1&amp;v=Z6mDcTnBmMA)

Les mises à jour se font lorsque le programme vous le dit, par téléchargement de l'APK. J'ai eu quelques soucis sur une version et je suis revenu avec du mal à la précédente. Donc laissez passer quelques jours avant la mise à jour, ça vaut mieux, parfois. Et gardez l'apk de la précédente tant que ce n'est pas complètement validé par votre utilisation. 

