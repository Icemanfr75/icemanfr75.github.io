---
layout: post
title: Tuto - Chiffrer (et pas crypter) et signer ses emails sur son smartphone ET son PC Windows
category: tuto
tags: android, chiffrement, clé, cryptage, email, gpg, K9mail, pgp, thunderbird, tutoriel
---
**Le Chiffrement (et pas le faux ami Cryptage) et la signature de mail deviennent une nécessité. Mais ce n'est pas si compliqué qu'il n'y paraît quand on fait les choses dans le bon ordre pour en profiter sur son PC comme sur son smartphone ...**

A lire maintenant sur : Tout d'abord, il vaut mieux commencer à créer sa clé GPG sur un PC...Mais je vais en venir d'abord aux notions pour la compréhension du principe.

### les notions de base

Signer un message revient à prouver l'authenticité de l'expéditeur à son destinataire. Chiffrer un message revient à le glisser dans une enveloppe ouverte uniquement par son destinataire. Pour faire cela avec un email donné, il faut créer des clés avec le logiciel GPG. La clé publique est celle que l'on diffuse à ses destinataires. La clé privée est celle que l'on garde pour chiffrer et/ou signer ses messages. Elle est sous la forme d'une suite de lettres ou de chiffres et peut (et doit) être sauvée dans un fichier ASCII. Il faut évidemment éviter d'utiliser GPG sur des comptes mail de sociétés qui n'hésitent pas utiliser les données de nos mails (Google, Microsoft, etc...)

### Configurer GPG sous Windows

En ce qui concerne les PC **sous windows**, inutile que je fasse un tutoriel car le Hollandais Volant en a un très bon : <a title="https://lehollandaisvolant.net/tuto/gpg/" href="https://lehollandaisvolant.net/tuto/gpg/">https://lehollandaisvolant.net/tuto/gpg/</a> . Il vous faudra donc deux logiciels : <a title="GPG4Win" href="http://www.gpg4win.org/">GPG4Win</a> et <a title="Thunderbird" href="https://www.mozilla.org/fr/thunderbird/">Thunderbird</a> avec son extension <a title="enigmail" href="https://addons.mozilla.org/en-US/thunderbird/addon/enigmail/">enigmail</a> (ou Clawsmail éventuellement).

Mais en ce qui concerne Android, GPG est un parent pauvre. Je propose de passer par le couple <a title="APG" href="https://play.google.com/store/apps/details?id=org.thialfihar.android.apg">APG</a> / <a title="K9-Mail" href="https://play.google.com/store/apps/details?id=com.fsck.k9">K9-Mail</a> ou bien <a title="OpenKeyChain" href="http://www.openkeychain.org/">OpenKeyChain</a> /K9-Mail, qui semble moins archaique dans sa forme . Mais tout d'abord, assurez vous d'avoir** votre clé privée **sauvegardée à partir de GPA/GPG4Win. Pour qu'elle soit lisible, il faut qu'en l'ouvrant avec le bloc note de votre windows, vous puissiez lire :

>-----BEGIN PGP PRIVATE KEY BLOCK-----
>
>et qu'il se termine par :
>
>-----END PGP PRIVATE KEY BLOCK-----

Vous aurez bien sur envoyé auparavant votre clé publique à vos correspondants, soit par fichier, soit en copiant le contenu du fichier ascii. Et donc il faut avoir le fichier de clé privée sur votre smartphone android.

### Configurer APG sous Android

Donc ouvrez APG (Qu'il faut installer impérativement AVANT K9-mail) dans votre android et accédez au menu en haut à gauche pour sélectionner "Importer les clefs". A la place de "serveur de clefs", sélectionnez "importer depuis un fichier" puis ouvrir et cherchez votre fichier. Normalement vous devez voir s'afficher une ligne avec "clef secrète : ...." avec votre pseudo, votre adresse mail et l'empreinte de la clé, une suite de 10 blocs de 4 caractère qui sert à vérifier l'authenticité. Il ne vous reste qu'à appuyer "importer les clefs choisies".

### Ou Configurer OpenKeyChain sous Android

Ouvrez OpenKeyChain et faites "import key from file", puis ouvrir pour aller chercher le fichier. Après validation, une ligne s'affiche avec le mail concerné et l'empreinte de la clé. Vous pouvez alors "importez les clés choisies".

Maintenant vous pourrez envoyer avec cette adresse sur votre smartphone. Mais vous ne savez pas lire les mails chiffrés par vos correspondants. Il vous faut importer leurs clés publiques de la même manière. Mais cette fois, vérifiez que le fichier commence par

>-----BEGIN PGP PUBLIC KEY BLOCK-----

### Une appli Mail adaptée

Pour un même compte mail (configuré en IMAP), vous pouvez donc chiffrer et signer vos mails avec la même clé et la diffuser avec vos correspondant. Pour cela, grace au client mail K9-Mail, il faudra évidemment installer le bon compte mail et le relier à APG. Normalement, K9 détecte automatiquement la présence d'APG mais il y a un bug qui fait apparaître 2 fois APG dans le menu Paramètres/Paramètres du compte/Cryptographie/Fournisseur OpenPGP. Il faut laisser sélectionné le APG sans clé dorée devant. Pour OpenKeyChain, il n'y a pas de souci.

Maintenant, vous pouvez choisir de signer systématiquement vos mails, voir les chiffrer pour les correspondants dont vous avez la clé publique, etc...

A noter que pour des mails chiffrés, il arrive que le message arrive en pièce attachée chiffrée au lieu d'être déchiffré automatiquement comme dans Thunderbird. Lors d'un envoi d'un mail chiffré, il faut aussi se souvenir que les pièces jointes ne sont pas chiffrées par défaut, donc attention à vérifier cela dans le client mail utilisé. Pour cela, vous pouvez essayer cette fonction en vous envoyant un mail sur une autre de vos adresses.

Si vous ne souhaitez pas utiliser K9-Mail, il reste possible d'envoyer des mails chiffrés directement depuis APG/OpenKeyChain qui partagera le message chiffréé dans votre appli habituelle. Mais elle ne sera qu'en pièce jointe ou comme bloc ascii dans le corps du message. Par contre il vous faudra faire des copier-coller des messages chiffrés reçus vers APG pour les décoder, ce qui est assez lourd, bien que très simple. APG a aussi des bugs dans sa gestion de fichier. Il faut passer par un gestionnaire de fichier après avoir sauvegardé la pièce jointe et ensuite l'envoyer "décrypter par APG" dans ce gestionnaire de fichier.

Enfin, idéalement, ne laissez pas votre clé privée accessible dans un répertoire facile d'accès. Avec la phrase/mot de passe à la création, c'est encore une protection à ne pas oublier

EDIT : On peut aussi faire le choix d'utiliser un produit comme Protonmail qui dispose maintenant d'une application.
