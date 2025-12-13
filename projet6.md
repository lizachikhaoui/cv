### Description de la version 6 de ce projet 
---
Cette veersion a été pour but d'intégrer les émotions et accompagner visuellement lecture de l'utilisateur par:

* La couleur de l'écran qui change en fonction du thème.

* Introduction de boutons thématiques correspondant à des émotions : Joie, Calme, Énergie, Douceur.

* Chaque bouton déclenche l’affichage d’un texte spécifique associé à l’émotion choisie.

* L’utilisateur peut réinitialiser l’état avec un bouton dédié(réinitialiser).

* Affichage et animation du texte: il s'affiche progressivement ligne par ligne, au lieu d’un affichage complet instantané.

* Chaque ligne change automatiquement après un intervalle de temps pour créer un effet de lecture rythmée.

* Effets visuels interactifs: Couleur de fond dynamique où chaque émotion a un gradient de couleurs spécifique.

* Particules flottantes créées autour du texte pour renforcer l’ambiance visuelle.

* Ondes lumineuses (cercles se dilatant au centre) pour un effet de “pulsation” correspondant à l’émotion.

* Gestion des transitions par l'utilisation de timeouts multiples pour synchroniser l’affichage du texte et les animations.

* Fonction resetEmotion() permettant de nettoyer l’écran, arrêter les animations et revenir au fond initial.

## En résumé:

* Affichage progressif du texte

* Utilisation de setTimeout pour afficher chaque ligne avec un délai (showLine).

* Gestion d’une liste de timers (timeoutList) pour pouvoir les annuler au reset.

2. Changement dynamique du fond

* Manipulation de document.body.style.background pour créer des dégradés selon l’émotion choisie.

* Transition CSS (transition: background 1s) pour un effet fluide.

3. Particules animées

* Création dynamique de div .particle via document.createElement.

* Positionnement aléatoire sur l’écran (style.left, style.top) et taille variable.

* Animation CSS via @keyframes float pour faire remonter et disparaître les particules.

* Suppression automatique avec setTimeout(() => p.remove(), 4000).

4. Ondes lumineuses pulsantes

* Création de div temporaire centrée.

* Animation via style.transform et style.opacity pour créer l’effet d’onde qui s’agrandit et disparaît.

* Suppression automatique après animation.

5. Réinitialisation

* Arrêt de tous les timers avec clearTimeout.

* Retour du texte et du fond à l’état initial.

