# 🌍 CampusZen

<div align="center">

**Application « Météo de l'état de bien-être »**

Une plateforme multilingue pour soutenir la santé mentale des étudiants en Afrique

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![Django](https://img.shields.io/badge/Django-4.2-green.svg)](https://www.djangoproject.com/)
[![React Native](https://img.shields.io/badge/React%20Native-0.81-61dafb.svg)](https://reactnative.dev/)
[![Expo](https://img.shields.io/badge/Expo-54.0-000.svg)](https://expo.dev/)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE)

</div>

## 📋 Table des matières

- [À propos du projet](#-à-propos-du-projet)
- [Demandeur](#-demandeur)
- [Contexte et objectifs](#-contexte-et-objectifs)
- [Objectifs qualitatifs](#-objectifs-qualitatifs)
- [Objectifs quantitatifs](#-objectifs-quantitatifs)
- [Architecture technique](#-architecture-technique)
- [Partenaires](#-partenaires)

## 🎯 À propos du projet

**CampusZen** est une application mobile innovante conçue pour aider les étudiants à suivre et améliorer leur bien-être mental au quotidien. Utilisant une interface intuitive basée sur une « météo émotionnelle », l'application propose un suivi personnalisé de l'état mental, des ressources localisées et une interface de mise en relation avec des professionnels.

## 👥 Demandeur

**Équipe projet Mama_Africa**

## 📍 Contexte et objectif

CampusZen s'inscrit dans le cadre du projet **Mama_Africa** dédié à la santé mentale des étudiants, avec un focus sur l'ampleur et la nature des troubles mentaux courants chez les étudiants ainsi que les barrières à l'accès aux soins.

### Zones de déploiement initial
- 🇸🇳 Sénégal
- 🇨🇲 Cameroun
- 🇨🇩 République Démocratique du Congo (RDC)
- 🇬🇭 Ghana
- 🇩🇿 Algérie

### Objectif principal

Fournir aux étudiants les outils ancrés dans les contextes **socio-économique, culturelle et politique** pour prendre soin de leur santé mentale au quotidien.

## ✅ Objectifs qualitatifs

- **Multilingue et accessible** : Français, Anglais et Arabe
- **Échelle du bien-être** : Outil de suivi émotionnel sous forme de « météo émotionnelle » (Ensoleillé ☀️, Nuageux ☁️, Orageux ⛈️) ou échelle de type Likert (très bien à très mal)
- **Messages d'encouragement** : Messages personnalisés en fonction de l'évaluation précédente pour encourager l'étudiant ou demander de l'aide
- **Cartographie des ressources** : Localisation des ressources existantes pertinentes (services médicaux, services sociaux, associations, etc.) avec évaluation du temps de trajet et des coûts d'accès depuis la localisation de l'étudiant

## 📊 Objectifs quantitatifs

- **Nombre d'utilisateurs attendus** : 10 000 étudiants au démarrage
- **Nombre de téléchargements** : 5 000 au démarrage

## 🚀 Fonctionnalités

### Interface utilisateur
- ✨ Interface simple, intuitive et conviviale
- ♿ Adaptation à tous les niveaux de littératie et aux personnes en situation de handicap (déficients visuels, auditifs, langage, troubles cognitifs, etc.)

### Multilinguisme
- 🌐 Support complet en Français, Anglais et Arabe

### Suivi du bien-être
- 📊 Suivi personnalisé de l'état de bien-être
- 📈 Échelles avec visualisations sous forme de graphiques ou icônes

### Ressources éducatives
- 📱 Articles, podcasts et vidéos sur la gestion du stress
- 💡 Stratégies pour améliorer le bien-être

## 🏗️ Architecture technique

### Structure du projet

```
CampusZen/
├── backend/                    # API REST Django
│   ├── campus_zen_backend/     # Configuration Django
│   ├── campusZen/              # Application principale
│   │   ├── models.py          # Modèles de données
│   │   ├── views.py           # Vues API
│   │   ├── serializers.py      # Sérialiseurs
│   │   ├── urls.py            # Routes
│   │   └── migrations/         # Migrations de base de données
│   └── requirements.txt        # Dépendances Python
│
├── frontend/                   # Application mobile React Native
│   └── campusZen/
│       ├── src/
│       │   ├── screens/        # Écrans de l'application
│       │   ├── components/     # Composants réutilisables
│       │   ├── services/       # Services API
│       │   ├── navigation/     # Navigation
│       │   ├── context/        # État global
│       │   ├── hooks/          # Hooks personnalisés
│       │   ├── theme/          # Thème de l'application
│       │   └── types/          # Types TypeScript
│       ├── package.json        # Dépendances Node.js
│       └── app.json            # Configuration Expo
│
└── module_admin/               # Interface d'administration Vue.js
    ├── src/
    │   ├── components/         # Composants Vue
    │   ├── views/              # Vues
    │   ├── router/             # Routage
    │   └── services/           # Services
    └── package.json            # Dépendances Node.js
```

### Stack technologique

#### Backend
- **Framework** : Django 4.2
- **API REST** : Django REST Framework (DRF) 3.16
- **Authentification** : JWT + Cookies HttpOnly
- **Base de données** : SQLite (développement) / PostgreSQL (production)
- **Serveur** : Gunicorn

#### Frontend Mobile
- **Framework** : React Native 0.81 avec Expo 54.0
- **Language** : TypeScript
- **Navigation** : React Navigation
- **State Management** : Context API + Hooks
- **Requêtes HTTP** : Axios
- **Stockage sécurisé** : Expo Secure Store
- **Localisation** : Expo Location
- **Graphiques** : React Native Chart Kit
- **Cartographie** : React Leaflet

#### Module Admin
- **Framework** : Vue.js 3
- **Build Tool** : Vite
- **Styling** : Tailwind CSS
- **Serveur** : Node.js avec Nginx

## 🏫 Partenaires

### Financement

**Agence Nationale de la Recherche** (ANR)

### Institutions gestionnaires

- **UMR PRODIG**
- **Institut de Recherche pour le Développement** (IRD)
- **Centre hospitalier Charles Perrens**

### Universités partenaires

Universités dans les zones de déploiement (Sénégal, Cameroun, RDC, Ghana, Algérie)

## Auteurs
- Enzo Familiar-Marais
- Matthias Caroux
- Niksan Nagarajah
- Samuel Niveau

## 📝 License

MIT - Voir [LICENSE](./LICENSE)
