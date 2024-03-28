# Utilisez une image Python comme base
FROM python:3.9

# Définissez le répertoire de travail dans le conteneur
WORKDIR /app

# Copiez les fichiers nécessaires pour l'installation des dépendances
COPY requirements.txt ./

# Installez les dépendances
RUN pip install --no-cache-dir -r requirements.txt

# Copiez le reste des fichiers de l'application
COPY . .

# Commande pour démarrer le service lorsque le conteneur est lancé
CMD ["python", "app.py"]
