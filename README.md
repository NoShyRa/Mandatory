# Mandatory

## À propos

* Ceci est un projet Docker pour WordPress avec Apache, PHP, MySQL et phpMyAdmin

&nbsp;

## Informations générales / Prérequis

**Prérequis :** docker, docker-compose

**Stack Docker :**

db = MySQL
wordpress = Apache, PHP
phpMyAdmin

&nbsp;

## Architecture du projet

- ./wordpress/: contient tout le code source de l'application WordPress et contient le fichier de sauvegarde initial de la base de données MySQL
- .env.sample: exemple à copier pour créer le fichier .env avec les identifiants de développement
- docker-compose.yml: configuration des conteneurs
- README: documentation de développement initiale du projet

&nbsp;

## Installation

### Variables d'environnement
Dans le cas où c'est la première initialisation du projet sur votre appareil :
1. `cp .env.sample .env`
2. Écrivez les variables dans ce fichier .env et choisissez leurs valeurs.

variables à configurer :
Network
Database
User
Password

par défaut :
Database= wordpress
User= wordpress
Password= wordpress
(password_root= password)

&nbsp;

### Docker

- Pour lancer la pile de développement Docker : `docker-compose up -d`
- Pour arrêter les conteneurs : `docker-compose stop` 
- Pour arrêter et supprimer les conteneurs et le réseau : `docker-compose down` 

