📦 Projet PHP - Gestion de Produits et Catégories
Ce projet est une application PHP simple pour gérer des produits et des catégories. Les fonctionnalités incluent l'ajout, la suppression et l'affichage de produits et de catégories.

⚙️ Fonctionnalités
Catégories
Ajouter une nouvelle catégorie.
Supprimer une catégorie existante.
Voir la liste des catégories.
Produits
Ajouter un nouveau produit avec une description, un prix, et une catégorie associée.
Supprimer un produit.
Voir la liste des produits par catégorie.
🛠 Installation
Cloner le dépôt ou télécharger les fichiers dans un dossier de votre serveur local (ex : le dossier www de WAMP).

Assurez-vous que votre serveur local (WAMP, XAMPP, etc.) est activé.

Créez une base de données nommée b2dev2 dans phpMyAdmin.

Importez la structure des tables (catégories et produits) dans la base de données b2dev2.

Structure de la base de données
Table categories :
id : INT, PRIMARY KEY, AUTO_INCREMENT
nom : VARCHAR(255)
Table produits :
id : INT, PRIMARY KEY, AUTO_INCREMENT
titre : VARCHAR(255)
description : TEXT
prix : DECIMAL(10,2)
categorie : INT, FOREIGN KEY vers categories.id
Vérifiez les informations de connexion à la base de données dans le fichier fonctions.php (hôte, utilisateur, mot de passe, nom de la base de données).

🚀 Utilisation
Accédez à l'application via http://localhost/votre_dossier.
Utilisez les onglets de navigation pour :
Ajouter une catégorie dans l'onglet "Catégories".
Ajouter des produits en les associant aux catégories dans l'onglet "Produits".
Consulter les listes des catégories et des produits par catégorie.
🗂 Structure des fichiers
index.php : Page d'accueil avec la liste des catégories.
categories.php : Page pour gérer les catégories (ajout et suppression).
produits.php : Page pour gérer les produits (ajout, suppression et affichage).
produits_par_categorie.php : Page pour afficher les produits par catégorie.
fonctions.php : Fichier de connexion à la base de données et des fonctions CRUD.
style.css : Fichier de style pour l'apparence de l'application.
