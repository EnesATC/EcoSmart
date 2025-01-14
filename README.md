EcoSmart - Gestion de Logement Éco-Responsable
EcoSmart est un projet étudiant conçu pour gérer les fonctionnalités d'un logement éco-responsable via une interface web intuitive et un serveur RESTful. Ce projet permet de surveiller, configurer et optimiser la consommation énergétique à l'aide de capteurs et d'actionneurs, tout en offrant des outils de visualisation et de gestion des factures.
--------------------------------------
Fonctionnalités
--------------------------------------
Configuration des Capteurs :
Ajout de capteurs/actionneurs dans différentes pièces.
Gestion des types de capteurs (température, humidité, consommation électrique, etc.).

État des Capteurs :
Affichage des capteurs installés avec leurs détails (type, localisation, port de communication).
Possibilité de supprimer un capteur existant.

Gestion des Factures :
Ajout de factures liées à la consommation (électricité, eau, gaz, déchets).
Affichage des factures existantes dans un tableau clair.
Suppression de factures directement depuis l'interface.

Visualisation de la Consommation :
Graphiques pour analyser la consommation en temps réel ou selon des périodes spécifiques (jour, semaine, mois, année).

Comparatifs Économiques :
Comparaison des consommations pour optimiser les dépenses.

-------------------------------------
Structure du Projet
-------------------------------------
1. Frontend
L'interface utilisateur est développée en HTML, CSS et JavaScript, avec des fichiers séparés pour chaque fonctionnalité.
Fichiers principaux :
index.html : Structure principale du site.
css/styles.css : Styles pour le design du site.
js/Configuration.js : Gestion de la configuration des capteurs.
js/capteurs.js : Affichage et gestion des capteurs.
js/consommation.js : Gestion des factures et affichage de la consommation.
js/ComparatifEconomique.js : Visualisation des comparatifs économiques.

2. Backend
Le serveur RESTful est développé avec FastAPI, et utilise une base de données SQLite pour stocker les données.
Fichiers principaux :
serveur_REST.py : Serveur RESTful pour gérer les requêtes (GET, POST, DELETE).
logement.db : Base de données SQLite contenant les informations sur les capteurs, mesures et factures.
logement.sql : Script SQL pour créer et remplir la base de données.
3. Base de Données

Les tables principales incluent :
Logement : Informations de base sur le logement.
Piece : Liste des pièces.
Type_Capteur_Actionneur : Types de capteurs/actionneurs.
Capteur_Actionneur : Liste des capteurs/actionneurs installés.
Mesure : Enregistrement des données des capteurs.
Facture : Gestion des factures énergétiques.
Prérequis

--------------------------------
Installation des dépendances :
--------------------------------
Python 3.x
Modules Python : fastapi, uvicorn, pydantic, sqlite3, cors

--------------------------------
Démarrage du serveur : 
--------------------------------
Lancer le serveur RESTful avec FastAPI 
Lancer le site web :
Ouvrir index.html dans un navigateur web.
Assurez-vous que le serveur REST est opérationnel sur http://127.0.0.1:8000.

--------------------------------
Fonctionnement
--------------------------------
Ajouter des Capteurs :
Naviguer dans la section Configuration.
Remplir les informations nécessaires et cliquer sur "Ajouter".

Consulter l'État des Capteurs :
Accéder à la section État des Capteurs.
Visualiser les capteurs installés et les supprimer si nécessaire.

Gérer les Factures :
Dans la section Consommation, ajouter de nouvelles factures via le tableau.
Supprimer des factures existantes directement.
Analyser les Consommations :

Visualiser les graphiques interactifs pour surveiller la consommation.

--------------------------------
Auteur et sources
--------------------------------
Enes ATICI - Projet réalisé dans le cadre d'un exercice étudiant. 
Les codes js sont proncipalement réalisé avec l'aide de ChatGPT. 
La base de données et le code du serveur ont été réalisé précédamment dans le cadre du cours IOT/SQL et adapté pour ce projet.
Les codes CSS et HTML ont été réalisé grace a un tutoriel youtube : https://www.youtube.com/watch?v=6hCGTJCo_Uo
La couleur verte a été pris du site : https://www.rolex.com/fr
Les images qui ont été utilisé lors de la réalisation du site ont été généré à partir d'une IA : DALL-E
