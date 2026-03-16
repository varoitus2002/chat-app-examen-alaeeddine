---

# Réponses Examen TT4

## Question 1 – Analyse du code

# App.js
App.js est le composant principal de l'application React. 
Il gère l'état global et décide si l'utilisateur voit Join.js ou Chat.js.

# Chat.js
Chat.js affiche l’interface principale du chat avec les messages et la zone pour envoyer un message.

# Message.js
Message.js sert à afficher chaque message dans la conversation avec son contenu et l’heure.

# Sidebar.js
Sidebar.js affiche les informations de la room et les utilisateurs connectés.

#Join.js
Join.js permet à l’utilisateur d’entrer son nom et la salle avant de rejoindre le chat.

# server.js
server.js est le serveur Node.js qui utilise Socket.io pour gérer les messages en temps réel.

#SocketContext.js
SocketContext.js permet de partager la connexion socket dans tous les composants React.

---

## Question 2 – Communication frontend/backend

### Création du socket
Le socket est créé dans SocketContext.js avec Socket.io puis partagé dans l’application grâce au Context API.

### Evènement rejoindre room
Quand un utilisateur rejoint une room, le client envoie un évènement `join_room` au serveur.

### Diffusion des messages
Le serveur reçoit le message et l’envoie à tous les utilisateurs de la room.

---

## Question 3 – Modification Message.js
Ajout d’un indicateur **Lu (✓✓)** sous les messages envoyés par l’utilisateur.

---

## Question 4 – Quitter la salle
Ajout d’un bouton permettant de quitter la room et revenir à Join.js.

---

## Question 5 – Historique des activités
Ajout d’un historique des connexions et déconnexions dans la sidebar.

---

## Amélioration
Une amélioration possible serait d’ajouter une base de données pour sauvegarder les messages.