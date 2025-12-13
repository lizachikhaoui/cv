### Description de la version 4 de mon peojet 
---
Cette version introduit une transformation importante de l’expérience utilisateur en combinant trois dimensions synchronisées :

* Lecture visuelle du texte

* Lecture vocale (Text-to-Speech)

* Musique d’ambiance en arrière-plan

L’application ne se limite plus à afficher ou lire un texte, mais propose désormais une expérience immersive de type “karaoké spirituel”, adaptée à la nature chantée des paroles chrétiennes.

En gardant les fonctionnalités de la version précédente, cette version guide le lecteur davantage dans sa lecture en sélectionnant la ligne de lecture (en jaune) sur laquelle est arrivé dans
le texte en la colorant en jaune. Lecture vocale synchronisée ligne par ligne,elle introduit une synchronisation entre voix et texte. Chaque ligne :

* Est lue individuellement.

* A un rythme contrôlé (rate = 0.9).

* Avec une intonation renforcée (pitch = 1.4) adaptée au chant.

Le texte est désormais affiché sous forme de lignes stylisées, avec une mise en évidence dynamique de la ligne en cours de lecture.
toutes les lignes sont visibles, seule la ligne active est mise en évidence et la progression suit la lecture vocale. Ce mécanisme guide visuellement le lecteur et renforce l’immersion.

Elle propose également un contrôle audio indépendant et avancé par l’utilisateur en intégrant des boutons:

* Pause : met en pause la voix
* Reprendre : relance la lecture vocale.
* Stop : réinitialise entièrement l’expérience

Ce système renforce le contrôle utilisateur et la stabilité de l’application.

Technologies utilisées :

HTML5 : 
* Structure et contrôles.

CSS3 :
* Styles karaoké.
* Transitions visuelles.
* Hiérarchisation du texte.

JavaScript ES6 :
* Gestion audio.
* Timers (setTimeout).
* Manipulation du DOM.

Web Speech API : synthèse vocale.
* Audio HTML5 : musique de fond.
