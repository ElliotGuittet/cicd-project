# Utilisez une image Node.js comme base
FROM node:14

# Définissez le répertoire de travail dans le conteneur
WORKDIR /app

# Copiez les fichiers nécessaires pour l'installation des dépendances
COPY package.json package-lock.json ./

# Installez les dépendances
RUN npm install

# Copiez le reste des fichiers de l'application
COPY . .

# Construisez l'application React pour la production
RUN npm run build

# Commande pour démarrer l'application lorsque le conteneur est lancé
CMD ["npm", "start"]
