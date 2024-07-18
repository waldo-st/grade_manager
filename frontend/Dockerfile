# Utiliser une image de base pour Node.js
FROM node:v20.12.2

# Définir le répertoire de travail
WORKDIR /app

# Copier les fichiers package.json et package-lock.json
COPY package*.json ./

# Installer les dépendances
RUN npm install

# Copier le reste de l'application
COPY . .

# Construire l'application
RUN npm run build

# Définir la commande de démarrage
CMD ["npm", "start"]
