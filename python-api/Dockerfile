# Récupérer une image de base pour python

FROM python:3.13-slim

WORKDIR /app

# Récupérer les dépendances

COPY requirements.txt .

RUN pip install -r requirements.txt

# Pour copier le contenu de java-api dans app

COPY . .

# Pour lancer l'application au démarrage du conteneur

CMD ["uvicorn", "src.main:app", "--host", "0.0.0.0", "--port", "8000"]