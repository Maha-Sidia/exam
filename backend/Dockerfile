# Utilise l'image officielle Node.js
FROM node:18

# Crée et se place dans le dossier de l'app
WORKDIR /app

# Copie package.json et package-lock.json si présent pour profiter du cache Docker
COPY package*.json ./

# Installe les dépendances
RUN npm install

# Copie tout le reste du code
COPY . .

# Expose le port sur lequel le serveur écoute
EXPOSE 3000

# Commande pour démarrer le serveur
CMD ["npm", "start"]

