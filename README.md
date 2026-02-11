# 🚗 Gestion du Parc Automobile - Zone Sanitaire ATZ

<div align="center">

![Version](https://img.shields.io/badge/version-2.0.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Status](https://img.shields.io/badge/status-production-success.svg)

**Application web de gestion du parc automobile pour la Zone Sanitaire Allada-Toffo-Zè (Bénin)**

[Démo](#-démarrage-rapide) • [Fonctionnalités](#-fonctionnalités) • [Installation](#-installation) • [Documentation](#-utilisation)

</div>

---

## 📋 Description

Cette application permet aux **36 centres de santé** de la Zone Sanitaire Allada-Toffo-Zè de déclarer et gérer leur parc automobile de manière centralisée. Elle offre une interface intuitive pour l'enregistrement des véhicules et un tableau de bord administratif complet pour le suivi.

## ✨ Fonctionnalités

### 👥 Pour les Centres de Santé
- ✅ Déclaration de véhicules (moto, voiture, ambulance, camion)
- ✅ Saisie des informations complètes (immatriculation, châssis, kilométrage, état)
- ✅ Validation des données en temps réel
- ✅ Notifications de confirmation

### 👨‍💼 Pour les Administrateurs
- 🔐 Accès sécurisé par code
- 📊 Tableau de bord avec statistiques en temps réel
- 🔍 Recherche et filtrage avancés
- ✏️ Modification et suppression des véhicules
- 📥 Export Excel et PDF
- 📋 Suivi des centres n'ayant pas encore déclaré

### 🎨 Interface Utilisateur
- 🌙 Design moderne et responsive
- 🎯 Modales élégantes (au lieu des alertes natives)
- 🔔 Notifications toast
- 📱 Compatible mobile et tablette

## 🚀 Démarrage Rapide

### Prérequis
- Un navigateur web moderne (Chrome, Firefox, Edge, Safari)
- Aucune installation côté serveur requise

### Installation

1. **Cloner le repository**
   ```bash
   git clone https://github.com/votre-username/gestion-vehicules-atz.git
   cd gestion-vehicules-atz
   ```

2. **Ouvrir l'application**
   - Double-cliquez sur `gestion_cs.html`
   - Ou servez avec un serveur local :
     ```bash
     # Avec Python
     python -m http.server 8000
     
     # Avec Node.js
     npx serve
     ```

3. **Accéder à l'application**
   - Ouvrez `http://localhost:8000` dans votre navigateur

## 📖 Utilisation

### Déclaration d'un Véhicule

1. Sélectionnez votre centre de santé
2. Remplissez les informations du véhicule
3. Cliquez sur "Enregistrer le Véhicule"

### Accès Administrateur

1. Cliquez sur "Espace Admin" dans l'en-tête
2. Entrez le code d'accès : `ATZ2025`
3. Accédez au tableau de bord complet

### Export des Données

- **Excel** : Génère un fichier `.xlsx` avec toutes les données
- **PDF** : Génère un rapport officiel formaté

## 🗂️ Structure du Projet

```
ATZ/
├── gestion_cs.html    # Application principale (HTML + CSS + JS)
├── README.md          # Documentation
├── LICENSE            # Licence MIT
└── .gitignore         # Fichiers à ignorer
```

## 🛠️ Technologies Utilisées

| Technologie | Usage |
|-------------|-------|
| HTML5 | Structure |
| CSS3 | Design responsive |
| JavaScript (ES6+) | Logique applicative |
| [Font Awesome](https://fontawesome.com) | Icônes |
| [Google Fonts (Inter)](https://fonts.google.com) | Typographie |
| [SheetJS (xlsx)](https://sheetjs.com) | Export Excel |
| [jsPDF](https://parall.ax/products/jspdf) | Export PDF |
| localStorage | Stockage des données |

## 🔒 Sécurité

> ⚠️ **Note importante** : Cette application utilise le stockage local (`localStorage`) du navigateur. Les données sont stockées côté client uniquement.

Pour une utilisation en production avec des données sensibles, il est recommandé de :
- Implémenter un backend avec base de données
- Ajouter une authentification sécurisée
- Utiliser HTTPS

## 📊 Centres de Santé Couverts

L'application couvre les 36 formations sanitaires de la Zone ATZ :

<details>
<summary>Voir la liste complète</summary>

| # | Centre | # | Centre |
|---|--------|---|--------|
| 1 | CS Adjan | 19 | CS Hinvi |
| 2 | CS Agbanou | 20 | CS Houègbo |
| 3 | CS Agon | 21 | CS Koundokpoé |
| 4 | CS Agué | 22 | CS Kpomè |
| 5 | CS Ahozonnoude | 23 | CS Lissegazoun |
| 6 | CS Ahouannonzoun | 24 | CS Lon Agonmey |
| 7 | CS Allada | 25 | CS Sedjedénou |
| 8 | CS Aota | 26 | CS Sékou |
| 9 | CS Attogon | 27 | CS Sey |
| 10 | CS Avakpa | 28 | CS Sèhouè |
| 11 | CS Ayou | 29 | CS Soyo |
| 12 | CS Colli | 30 | CS Tangbo |
| 13 | CS Coussi | 31 | CS Toffo Centre |
| 14 | CS Dame | 32 | CS Togoudo |
| 15 | CS Dawé | 33 | CS Topka |
| 16 | CS Djanglanme | 34 | CS Zè |
| 17 | CS Djigbé-Agué | 35 | Bureau de Zone ATZ |
| 18 | CS Dodji-Bata | 36 | Hôpital de Zone Allada-Toffo-Zè |

</details>

## 🤝 Contribution

Les contributions sont les bienvenues ! Pour contribuer :

1. Forkez le projet
2. Créez une branche (`git checkout -b feature/amelioration`)
3. Committez vos changements (`git commit -m 'Ajout d'une fonctionnalité'`)
4. Pushez sur la branche (`git push origin feature/amelioration`)
5. Ouvrez une Pull Request

## 📝 Changelog

### v2.0.0 (2025)
- ✨ Refonte complète de l'interface utilisateur
- 🎨 Nouveau design moderne et responsive
- ➕ Ajout des fonctionnalités d'édition et suppression
- 🔍 Recherche et filtrage des véhicules
- 🔔 Système de notifications toast
- 📊 Statistiques améliorées (véhicules en mauvais état)
- 📄 Export PDF amélioré (format paysage, pagination)
- ⛽ Ajout du champ "Carburant"

### v1.0.0 (2024)
- 🚀 Version initiale
- 📝 Formulaire de déclaration
- 👨‍💼 Espace administrateur
- 📥 Export Excel et PDF

## 📄 Licence

Ce projet est sous licence MIT. Voir le fichier [LICENSE](LICENSE) pour plus de détails.

## 📧 Contact

**Zone Sanitaire Allada-Toffo-Zè**  
Ministère de la Santé - République du Bénin

---

<div align="center">

Développé avec ❤️ pour la santé publique au Bénin

</div>
