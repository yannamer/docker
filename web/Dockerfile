# Utiliser une image Python comme base
FROM python:3.7-slim

# Créer le répertoire de travail dans le conteneur
WORKDIR /app

# Copier les fichiers nécessaires dans le conteneur
COPY requirements.txt /app/
RUN pip install --no-cache-dir -r requirements.txt

# Copier le reste du code source (HTML, CSS, Python, etc.)
COPY . /app

# Exposer le port 5000 (Flask utilise généralement ce port)
EXPOSE 5000

# Démarrer l'application Python
ENTRYPOINT ["python", "app.py"]
