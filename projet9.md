### Description de la version 9 de mon projet
---
Cette version vise à ajouter des fonctionnalités diverses:
1. Musique de fond intégrée

* Ajout d’une musique relaxante en arrière-plan :

* const music = new Audio("...").
* music.loop = true.
* music.volume = 0.5.

La musique est pensée pour renforcer l’expérience spirituelle et immersive.

 2. Contrôles de la musique (nouveaux boutons)

3 nouveaux boutons dans l’interface :

* Pause musique

* Reprendre musique

* Stop musique


3. Fonctions JavaScript associées :

* pauseMusic()
* resumeMusic()
* stopMusic()

4. Gestion du son améliorée

Possibilité de :

* mettre en pause sans perdre la position

* reprendre la lecture

* arrêter complètement et revenir au début


* Volume réglé par défaut (0.5) pour rester doux et non agressif.

flowchart TD
    A[Chargement de la page HTML] --> B[Chargement du CSS et du DOM]
    B --> C[Initialisation du script JavaScript]

    C --> D[Création de l'objet Audio]
    D --> E[Initialisation des variables\nchant, colors, timeoutList]

    E --> F[Affichage du texte par défaut\n"Choisis une ambiance émotionnelle"]

    F --> G{Action utilisateur}

    %% ----------- CHOIX EMOTION -----------
    G -->|Clic bouton émotion| H[playEmotion(type)]
    H --> I[resetEmotion()]
    I --> J[Changement du fond selon l'émotion]
    J --> K[Initialisation index i = 0]

    K --> L{i < longueur du chant ?}
    L -->|Oui| M[Afficher lignes du chant]
    M --> N[Créer particules colorées]
    N --> O[Créer onde lumineuse]
    O --> P[setTimeout 2s → ligne suivante]
    P --> L
    L -->|Non| F

    %% ----------- RESET -----------
    G -->|Clic Réinitialiser| R[resetEmotion()]
    R --> S[Arrêt des timeouts]
    S --> T[Réinitialisation du texte]
    T --> U[Réinitialisation du fond]

    %% ----------- MUSIQUE -----------
    G -->|Pause musique| V[pauseMusic()]
    G -->|Reprendre musique| W[resumeMusic()]
    G -->|Stop musique| X[stopMusic()]

    %% ----------- MOUVEMENT SOURIS -----------
    C --> Y[Écouteur mousemove]
    Y --> Z[Création traînée lumineuse]
    Z --> AA[Animation + suppression après 1s]

    ## Diagramme de flux disponible sur le repository "diagramme"

    # Les IAG utilisés: Gemini pour la visualisation d'exemple et l'aide dans le code

    J'ai utilisé les sources techniques fourni par le professeur: https://docs.mermaidchart.com/mermaid-oss/syntax/flowchart.html ...

    Exemple de prompts: Comment fonctionne l’API fetch en JavaScript pour appeler une API de traduction ?
    Génère un exemple de code JavaScript qui découpe un texte en mots cliquables.



