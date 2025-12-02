#  Projet de Codage : Lecture Assistée Bilingue (L.A.B.)

## Idée du projet :
Créer une interface web de lecture de livres français où l'utilisateur peut **cliquer sur n'importe quel mot pour afficher sa traduction instantanée** (vers l'anglais, par exemple).

Ce projet vise à améliorer l'accessibilité des textes et à fluidifier l'apprentissage du vocabulaire en contexte.

---

## Objectifs et Réalisation Technique :

| Objectif | Technique Clé | Rôle de anime.js |
| :--- | :--- | :--- |
| **Rendre le texte interactif** | Manipulation du **DOM** (JavaScript) | Non applicable. |
| **Traduire en temps réel** | Requêtes **Asynchrones (fetch)** vers une API de traduction publique. | Non applicable. |
| **Amélioration de l'UX/UI** | **anime.js** | Animation fluide de l'apparition et de la disparition du *tooltip* (fondu + glissement). Animation de feedback visuel (zoom) sur le mot cliqué. |

---

## Technologies Utilisées :

* **HTML & CSS** : Structure du livre et style de lecture minimaliste.
* **JavaScript (ES6+)** : Logique de la décomposition du texte en mots cliquables et gestion des événements.
* **Librairie anime.js** : Moteur d'animation pour les transitions du *tooltip*.
* **API de Traduction** : Appel API externe pour obtenir la traduction en ligne.
