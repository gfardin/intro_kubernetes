TP1

# Ma procédure

- importer et décompresser les fichiers python et java api
- créer deux Dockerfile :
    - dans python-api, utilise une image de base pour python et ajoute le chargement des dépendances (avant de charger l'app pour des raisons de rapidité), et l'api avec uvicorn
    - dans java-api, qui sépare la partie jdk pour le build et la partie jde qui contient le jar (fichier compilé pour l'exécution)
- générer des images à partir de ces dockerfiles et les push sur DockerHub
- manipuler des conteneurs en local, crées à partir des images

# Mes difficultés

- j'ai oublié l'import des dépendances dans la partie python
- initialement au lancement d'un conteneur python j'éxectutais le main sans uvicorn (pas de port exposé)
- partie sur java : je n'avais pas compris ce qu'il fallait ajouter à chaque stage

# Mes remarques

- Docker permet de créer une image de notre application
- Un conteneur faisant tourner cette image peut fonctionner dans tout type d'environment
- un peu de mal à saisir la notion de compilation en java