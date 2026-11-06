# TP1 – Git et Python

## Présentation

**Nom du TP :** TP1 – Découverte de Git, GitHub et Python (dépôt `tp_git_python`).

**Objectif du programme :** `main.py` est un petit programme Python qui
s'utilise dans le terminal. Il accueille l'utilisateur, lui demande son prénom,
la matière qu'il veut réviser et la durée de sa séance, puis affiche un objectif
de révision personnalisé. Le but du TP n'est pas la complexité du code, mais
l'apprentissage du travail avec Git et GitHub.

**Rôle du fichier `main.py` :** c'est le fichier principal et unique du projet.
Il contient tout le code et c'est lui que l'on exécute. Il a évolué en quatre
versions, en ajoutant des instructions à chaque fois sans supprimer les
précédentes.

## Évolution du programme

| Version | Évolution de `main.py` |
|---------|------------------------|
| V1 | Création locale du programme avec un simple message de bienvenue. |
| V2 | Ajout de la saisie du prénom de l'utilisateur. Cette version a été envoyée sur GitHub avec le premier `git push`. |
| V3 | Ajout de la matière à réviser, modifié directement sur GitHub. Le changement a ensuite été récupéré sur le PC avec `git pull`. |
| V4 | Ajout de la durée de révision (en minutes), faite sur le PC, puis publiée avec un nouveau `git push`. |

## Utilisation

**Outils nécessaires :**
- Python 3 installé (vérification : `py --version`)
- Git (pour cloner le dépôt)
- Un terminal (par exemple Git Bash ou le terminal de VS Code)

**Étapes pour lancer le programme :**

1. Cloner le dépôt et entrer dans le dossier :

```
git clone https://github.com/Guesmiminyar/tp_git_python.git
cd tp_git_python
```

2. Lancer le programme :

```
py main.py
```

(Sur Linux ou macOS : `python3 main.py`.)

**Informations demandées à l'utilisateur :**
- son prénom ;
- la matière qu'il veut réviser ;
- la durée de la séance, en minutes.

À la fin, le programme affiche l'objectif, par exemple :
`Objectif : reviser maths pendant 30 minutes.`

## Commandes Git utilisées

| Commande | Rôle pendant le TP1 |
|----------|---------------------|
| `git init` | Initialise le dépôt Git local dans le dossier du projet. |
| `git add` | Place les fichiers modifiés (ici `main.py`) dans la zone d'index, pour qu'ils soient inclus dans le prochain commit. |
| `git commit` | Enregistre une version du projet avec un message (V1, V2, V3, V4). |
| `git push` | Envoie les commits locaux vers le dépôt GitHub. |
| `git pull` | Récupère sur le PC les modifications faites sur GitHub (utilisé pour V3). |