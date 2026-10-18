# Confidentialité de Filigrane mes documents

**En bref : vos documents ne quittent pas votre ordinateur.** Pas de compte, pas de cloud, pas de télémétrie, pas
de publicité, pas de mise à jour automatique.

## Ce que le logiciel envoie sur Internet

Rien. Au démarrage, le logiciel coupe lui-même toute connexion réseau dans son propre programme : même par erreur, il
ne pourrait rien envoyer. Son code source est visible pour que chacun puisse le vérifier.

Deux actions ouvrent un autre programme, seulement quand vous cliquez : l'adresse de contact (votre logiciel de
messagerie) et, le cas échéant, une page web (votre navigateur).

## Mises à jour : seulement si vous le demandez

Le logiciel ne vérifie jamais seul s'il existe une version plus récente. Si vous choisissez Aide › Vérifier les mises
à jour et répondez « Oui » au message qui s'affiche, il se connecte à GitHub (api.github.com), et à lui seul, pour lire
le numéro de la dernière version publiée. Il envoie le nom et la version du logiciel, comme toute demande à un site ;
GitHub voit votre adresse IP. Aucun document, nom, destinataire ni historique n'est envoyé. La connexion est ouverte le
temps de cette vérification, puis refermée.

## Fichiers Word, OpenDocument et texte

Pour ces fichiers, le logiciel demande à Microsoft Word ou à LibreOffice, s'ils sont installés sur votre ordinateur,
de les convertir en PDF. Cette conversion se fait sur votre ordinateur. Word et LibreOffice sont des programmes
séparés, soumis à leurs propres réglages : selon ceux-ci, ils peuvent par exemple charger une image liée à un
document depuis Internet. Les PDF et les photos n'utilisent ni Word ni LibreOffice.

## Ce qui est enregistré sur votre ordinateur

| Fichier | Contenu | Comment l'effacer |
|---|---|---|
| `.filigrane_mes_documents.json` (dossier personnel) | réglages d'apparence : couleur, opacité, taille, thème | supprimer le fichier |
| `.filigrane_mes_documents_historique.json` (dossier personnel) | historique : date, destinataire, motif et emplacement des copies | bouton « Effacer l'historique » du volet, ou supprimer le fichier |

Le texte du filigrane n'est jamais enregistré dans les réglages. Sous Linux, l'historique n'est lisible que par vous.
Les fichiers temporaires d'une conversion sont supprimés dès qu'elle est terminée.

## Les copies filigranées

Le filigrane fait partie de l'image : il ne s'enlève pas comme un calque. Les informations cachées du fichier
d'origine (position GPS d'une photo, appareil, auteur, titre) sont retirées. La copie ne porte ni le nom de l'éditeur
ni celui du logiciel. Son nom proposé reprend celui de l'original suivi de `_filigrane` : vous pouvez le changer au
moment d'enregistrer.

Un filigrane rend la réutilisation frauduleuse d'une copie plus difficile et plus visible ; il ne peut pas l'empêcher
dans tous les cas. Gardez vos originaux.

## Contact

Anthony BELKACEM EI, 200 rue de la Croix Nivert, 75015 Paris. Questions : apps@belkacem.fr
