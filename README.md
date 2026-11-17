# opsh : mini-shell en Python

Projet 2 du cours de Systèmes d'Exploitation.

## Description

opsh est un petit interpréteur de commandes écrit en Python. Il lit une
commande, crée un processus fils avec fork, l'exécute avec exec et attend sa
fin avec waitpid. Plusieurs commandes peuvent être reliées avec `->` : la
sortie de chaque commande devient l'entrée de la suivante.

## Fonctionnalités

- boucle de lecture avec l'invite `opsh>`
- chaînage de commandes avec `->`
- commandes internes `cd` et `exit`
- message d'erreur si la commande est introuvable

## Exécution

Prérequis : Linux (ou WSL) avec Python 3.

    git clone https://github.com/ibtissammm-hub/projet-final.git
    cd projet-final
    python3 code/opsh

## Exemples

    opsh> ls
    opsh> ls -> wc -l
    opsh> cd ..
    opsh> exit

## Contenu du dépôt

- `code/` : code source
- `report.pdf` : rapport
- `demo.mp4` : vidéo de démonstration
