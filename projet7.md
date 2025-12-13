### Descripion de ma version 7 de ce projet 
---
Affichage progressif d’un chant complet :

* Au lieu d’afficher seulement des phrases par émotion, maintenant tout le chant (“Chant joyeux”) est affiché ligne par ligne.

* Les lignes sont concaténées et séparées par des sauts de ligne (\n).

Ambiances émotionnelles appliquées au chant :

* Chaque type d’émotion (joie, calme, énergie, douceur) change le dégradé de fond de la page.

* Animations visuelles en parallèle :

* Particules flottantes qui apparaissent autour de l’écran.

* Ondes lumineuses centrales qui s’agrandissent et disparaissent pour accentuer le rythme.

Bouton de réinitialisation :

* Permet d’arrêter le chant et les animations et de revenir à l’état initial.

## Les techniques utilisées:
* Affichage progressif ligne par ligne

* Utilisation de setTimeout pour afficher chaque ligne avec un délai (ici 2000 ms).

* La variable timeoutList garde la trace de tous les timers pour pouvoir les annuler avec clearTimeout.

* Manipulation dynamique du DOM

* Document.body.style.background pour changer le dégradé selon l’émotion.

* innerHTML mis à jour avec chant.slice(0, i + 1).join("\n") pour accumuler les lignes.

Création d’éléments visuels dynamiques

Particules : 
* Création de div .particle avec position et taille aléatoires. Animation via @keyframes float.

* Ondes lumineuses : div centrée transformée et agrandie avec transform: scale() et opacity.

* Gestion des animations et reset

* Suppression automatique des éléments créés (p.remove() et wave.remove()).

* Annulation des timers et remise à zéro du texte et du fond via la fonction resetEmotion().

* Timers pour affichage progressif

* setTimeout pour afficher les lignes du chant avec un intervalle fixe.

* timeoutList pour stocker et annuler ces timers si nécessaire.

Manipulation dynamique du DOM

innerHTML pour afficher le texte du chant ligne par ligne.

document.body.style.background pour changer le fond selon l’émotion.

Animations dynamiques

* Particules : div créées avec positions et tailles aléatoires, animées via @keyframes float.

* Ondes lumineuses : div centrée avec transformation scale() et transition de opacity.

Gestion du reset

* clearTimeout() pour arrêter l’affichage progressif.

* Suppression des éléments DOM générés pour les animations.

* Remise à zéro du texte et du fond.

[Utilisateur clique sur un bouton émotion]
                  │
                  ▼
        playEmotion(type)      ──► change le dégradé du fond selon 'type'
                  │
                  ▼
      Réinitialise l'affichage
        ┌─────────────────────────┐
        │ resetEmotion()          │
        │ - Annule les timeouts   │
        │ - Réinitialise texte   │
        │ - Remet le fond initial│
        └─────────────────────────┘
                  │
                  ▼
      Affichage progressif des lignes
        ┌──────────────────────────────┐
        │ setTimeout(showLine, 2000)  │
        │ - Affiche chant[0..i]       │
        │ - Incrémente i               │
        └──────────────────────────────┘
                  │
                  ▼
    Création d’animations pour chaque ligne
       ┌──────────────────────────────┐
       │ createParticles(color)      │  ─► génère div flottantes
       │ createWave(color)           │  ─► cercle central qui s’agrandit
       └──────────────────────────────┘
                  │
                  ▼
    Répète jusqu’à la fin du chant
                  │
                  ▼
          [Chant complet affiché]
