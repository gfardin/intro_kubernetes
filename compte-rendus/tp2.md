TP2

# Ma procédure

- Création d'un manifest Yaml permettant de créer un déploiement de 3 pods
- Les pods suivent un template et contiennent un conteneur basé sur l'image stockée sur Dockerhub du tp1
- On crée le deployment avec kubectl
- On teste qu'il fonctionne en recherchant l'IP des PODs et en effectuant des requêtes api

# Mes difficultés

- Comprendre que le selector fait correspondre les pods que le deployment crée avec un template de pods via un label
- Voir que la requête doit mentionner un port de destination en plus de l'IP

# Mes remarques

- Un manifest permet de déployer des pods qui contiennent notre app via un conteneur
- Pas facile de trouver tous les éléments à mettre dans le Yaml