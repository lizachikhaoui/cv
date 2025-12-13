### Description de la version 5 de mon projet 
---
Cette nouvelle version intègre désormais une lecture mot par mot, où chaque mot est synchronisé avec une synthèse vocale en temps réel. Cette granularité fine améliore la compréhension,
l’attention et l’immersion du lecteur.
L’expérience utilisateur a été enrichie par des options de personnalisation avancées :

* Choix de la voix de synthèse vocale.

* Contrôle de la vitesse de lecture.

* Activation d’un mode nuit pour le confort visuel.

Sur le plan technique, le projet exploite désormais les Web Speech API pour la lecture vocale et la Web Audio API pour analyser la musique d’ambiance. Cette analyse sonore alimente un
visualiseur audio dynamique affiché sur un canvas, ajoutant une dimension visuelle réactive au son.

Cependant, l’utilisateur ne se contente plus seulement de lire mais il interagit, configure et accompagne le chant dans une expérience immersive où texte, voix, musique et animation sont
étroitement synchronisés.
En conclusion, Chants joyeux est passé d’un simple lecteur de textes à une plateforme interactive immersive, illustrant une maîtrise progressive des technologies web modernes (DOM, audio,
synthèse vocale, canvas) et une réflexion avancée sur l’ergonomie, l’accessibilité et l’expérience utilisateur.

L'espace de lecture a été agrandi pour plus de lisibilité avec u texte indiquand que l'utilisateur est libre de cliquer sur le chant qu'il veutfaire afficher et c'est à lui de décider
quand est-ce qu'il veut commencerLe, il sera ensuite redirigé vers un  système de boutons qui joue un rôle central dans l’interaction utilisateur, en permettant la sélection dynamique
de différents chants. Chaque bouton correspond à un identifiant unique qui référence un texte spécifique stocké en JavaScript. Lorsqu’un utilisateur clique sur un bouton, le texte associé
est injecté dans la zone d’affichage sous forme de mots individuels (<span>), permettant la mise en évidence mot par mot, la lecture audio synchronisée et la coordination avec la musique
de fond. Ce mécanisme assure une navigation fluide entre les chants, optimisant l’expérience utilisateur tout en garantissant la synchronisation entre l’affichage et les fonctionnalités
audio-visuelles.
Ainsi, il peut également cliquer sur les boutons( pause, reprendre, stop) pour faire marcher le texte ou l'arrêter.
