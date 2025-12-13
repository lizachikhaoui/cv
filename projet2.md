###  Description de la version 2  de mon projet 
---
Dans cette version le lecteur est orienté sur l'interface comme ceci: 
---
*  Cliquez sur le texte affiché d  ans l'interface( cliquez sur le bouton pour commencer)ces derniers qui sont des clés de sections précises.
*  Clic sur le bouton bleu ci-dessous: grand dieu pour lire les strophes appelées ici grand dieu.
*  Clic sur le bouton bleu ci-dessous: Appelez pour lire le texte intitulé ici appelez.
*  Clic sur le bouton bleu: Jésus pour lire le texte de Jésus.

Cette version est dédiée à la lecture interactive de chants chrétiens. Elle vise à proposer une expérience de lecture structurée, fluide et progressive, mettant en valeur le texte par une présentation rythmée et animée.
L’objectif principal est de faciliter la lecture contemplative, en laissant à l’utilisateur le contrôle du contenu affiché via une interface simple et intuitive.

L'architecture repose sur un epage html simple organisé autour d'un conteneur central par un titre servant de repère sémantique, d'une zone de lecture contenant l'affichage du texte et le guide pour commenez la lecture (cliquez sur un bouton pour commencer) et d'un conteneur de boutons qui se génère automatiquement.
Les chants sont stockés dans un objet JavaScript structuré, chaque clé correspondant à une section ou un chant :grand dieu [Grand dieu puissant, nous célébrons]...

Chaque chant est découpé en lignes indépendantes, ce qui permet :
----
* Un affichage progressif des strophes.
* un contrôle précis du rythme de lecture.
* Une extensibilité simple (ajout de chants sans modifier la logique).

Finalement, Les boutons de sélection des chants sont générés automatiquement à partir des clés de l’objet texts (script.js) pour adapter automatiquement l'interface à l'évolution du contenu.
