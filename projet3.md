### Description de la version 3  de mon projet 
---
Cette nouvelle version de projet: Chants joyeux marque une évolution fonctionnelle significative du projet en intégrant une dimension audio à l’expérience de lecture. L’application
ne se limite plus à l’affichage progressif des textes mais elle propose désormais une lecture vocale synchronisée avec l’apparition des lignes de texte, transformant l’outil de lecture en
une expérience multimodale (visuelle et sonore).

Nouvelle fonctionnalité principale : la lecture audio générée par(Text-to-Speech)

Cependant, la principale nouveauté introduite dans cette version est l’utilisation de l’API Web Speech (SpeechSynthesis) intégrée aux navigateurs modernes qui permet:

* Une lecture vocale en français (fr-FR).

* un débit de parole légèrement ralenti pour améliorer l’intelligibilité.

* Une intonation neutre adaptée à un texte spirituel.

* La lecture est déclenchée ligne par ligne, en synchronisation avec l’affichage visuel.

De plus, la synchronisation texte – audio a été efficace par la génération d ela fonction showText() pour coordoner: l’apparition progressive des lignes et la lecture vocale correspondante.
Chaque ligne est lue après un délai calculé à partir de son index(voir le code à la ligne , ce qui permet: de respecter le rythme de lecture et d’éviter les superpositions audio et
d’accompagner visuellement l’utilisateur pendant l’écoute, cette synchronisation renforce le caractère immersif et guidé de l’expérience.

Une gestion explicite de l’état de la synthèse vocale a été ajoutée pour améliorer la robustesse fonctionnelle de l’application: speechSynthesis.cancel() cette instruction garantit que :

* Toute lecture en cours est arrêtée lorsqu’un nouveau chant est sélectionné,

* Les chevauchements de voix sont évités,

* L’application reste cohérente lors d’interactions rapides.

Technologies utilisées dans cette version
---
1 HTML5 : 
          * Structure sémantique de l’interface.

2 CSS3 :
          * Animations (@keyframes)

          * Mise en page responsive.
3 JavaScript ES6 :

          * Manipulation du DOM,

          * Gestion des délais (setTimeout),

          * Contrôle de la synthèse vocale.

4 Web Speech API (SpeechSynthesis) :

* Lecture audio intégrée.
