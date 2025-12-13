### Description de la version 1 de mon projet 
---
A ce stade, j'ai changé de contenu pour mon projet (intégration des textes structurés de "champs joyeux" téléchargé en fichier csv ) tout en conservant sa structure technique de base pour un affichage dynamique du texte et une logique de changement du contenu en tant que lecteur sans avoir besoin de charger la page à chaque fois mais en cliquant sur "changer le texte" situé en dessous du texte initial. Des données qui ont été exploitées côté javascript pour afficher les strophes phrase par phrase.

Cela permet donc une lecture non seulement dynamique mais aussi interactive en lisant le texte phrase par phrase, ce qui nous laisse le temps de prendre de pauses quand 
on veut et s'arrêter sur le passage qu'on veut et contrôler le rythme d'affichage comme on le souhaite.

Ceci est également différent de la version précédente car il permet la séparation entre les données originales (le texte) et les logiques d'affichage( l'option : changer de texte).
Et enfin, on a rajouté une fonction( masquer traduction) pour cacher la traduction qui s'affichait au départ et on a utilisé anime.js pour arrêter toutes les animations qui s'affichent par tooltip, et on a lancé une nouvelle animation.js qui dure 200 millisecondes avec une précision de quel élement html sera animé (targets: tooltip), ce dernier qui devient invisible progressivement (opacity 0) et le groupe s'exécute une fois l'animation est terminée).
