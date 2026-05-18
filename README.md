# 🏃 Gestion de Courses Sportives — PHP MVC

> Application web complète avec architecture MVC pour la gestion d'événements sportifs  
> Projet académique — ESA Namur, Belgique | 2ème année Bachelier Informatique

[![PHP](https://img.shields.io/badge/PHP-8.x-777BB4?style=flat&logo=php&logoColor=white)](https://php.net)
[![SQLite](https://img.shields.io/badge/SQLite-3-003B57?style=flat&logo=sqlite&logoColor=white)](https://sqlite.org)
[![MVC](https://img.shields.io/badge/Architecture-MVC-green?style=flat)](https://fr.wikipedia.org/wiki/Mod%C3%A8le-vue-contr%C3%B4leur)
[![Composer](https://img.shields.io/badge/Composer-dependency%20manager-885630?style=flat&logo=composer)](https://getcomposer.org)
[![Portfolio](https://img.shields.io/badge/Portfolio-eamc.fr-c9a84c?style=flat)](https://eamc.fr)

---

## 📋 Description

Application web PHP complète pour la **gestion d'événements sportifs** (courses, trails, cyclisme). Elle comprend une partie publique pour les inscriptions en ligne et un **panel d'administration complet** pour gérer les événements, catégories et participants.

---

## ✨ Fonctionnalités

### 🌐 Interface publique
- Page d'accueil avec liste des événements disponibles
- Formulaire d'inscription en ligne complet
- Sélection de catégorie, taille t-shirt, mode de paiement
- Gestion du code UCI (cyclisme)

### 🔐 Panel d'administration
- Authentification sécurisée (login/sessions/logout)
- Gestion des événements sportifs (CRUD)
- Gestion des catégories par course
- Gestion des participants inscrits
- Attribution des dossards
- Suivi des paiements

---

## 🏗️ Architecture MVC

```
gestion-courses-php/
├── public/              # Point d'entrée web
│   └── index.php
├── src/
│   ├── models/          # Accès aux données (SQLite)
│   ├── views/           # Templates HTML
│   └── controllers/     # Logique métier
├── vendor/              # Dépendances Composer
├── composer.json
└── README.md
```

---

## 🗄️ Base de données SQLite

4 tables principales :

| Table | Description |
|---|---|
| `users` | Comptes administrateurs |
| `events` | Événements sportifs |
| `categories` | Catégories par événement |
| `participants` | Inscriptions des coureurs |

---

## 🧠 Concepts PHP utilisés

| Concept | Utilisation |
|---|---|
| Architecture MVC | Séparation Models / Views / Controllers |
| PDO + SQLite | Accès sécurisé à la base de données |
| Sessions PHP | Authentification et sécurité |
| Composer | Gestion des dépendances |
| Symfony var-dumper | Debug et développement |
| Formulaires POST | Inscriptions et administration |
| Prepared statements | Protection contre les injections SQL |

---

## 🚀 Installation

### Prérequis
- PHP 8.x
- Composer
- Serveur web (Apache/Nginx) ou `php -S`

### Installation

```bash
# Cloner le repository
git clone https://github.com/alfred17106/gestion-courses-php.git

# Aller dans le dossier
cd gestion-courses-php

# Installer les dépendances
composer install

# Lancer le serveur de développement
php -S localhost:8000 -t public/
```

Ouvrir `http://localhost:8000` dans votre navigateur.

---

## 👨‍💻 Auteur

**Ekolle Alfred Mbondo Céleste**  
Étudiant en Bachelier Informatique — ESA Namur, Belgique  
Licence en Informatique Fondamentale — Université de Douala, Cameroun

🌐 [eamc.fr](https://eamc.fr) · 📧 [alfred@eamc.fr](mailto:alfred@eamc.fr) · 🐙 [GitHub](https://github.com/alfred17106)

---

*Projet académique — ESA Namur 2024-2025*
