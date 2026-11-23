Debug Lab 1

On requête plusieurs fois le service créé. On se rend compte qu'il renvoie une erreur ou non de manière aléatoire, ce qui s'explique par un double problème :
    - Le deployment beta écoute sur 8080 alors que le service vise 5678
    - Le service pointe vers mon-api, or les pods des deux deployment s'appelent mon-api. Résultat, il requête aléatoirement un pod de alpha ou un de beta.
Si la requête aléatoire touche beta, il y a une erreur, sinon non.