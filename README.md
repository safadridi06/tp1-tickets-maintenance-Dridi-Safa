# TP1 – Gestion des tickets de maintenance

## 1. Identité

- **Nom et prénom :** SAFA DRIDI
- **Établissement :** ISET Djerba
- **Classe :** 2ème année – Développement des Systèmes d'Information
- **Module :** ATELIER FRAMEWORK COTE CLIENT

## 2. Prérequis

- Node.js
- npm
- Visual Studio Code
- Navigateur Web

## 3. Installation

Cloner le dépôt GitHub :

```bash
git https://github.com/safadridi06/tp1-tickets-maintenance-Dridi-Safa
```

Accéder au dossier du projet :

```bash
cd tickets-maintenance
```

Installer les dépendances :

```bash
npm install
```

## 4. Lancement du projet

### Lancement du serveur JSON

Dans un premier terminal :

```bash
npx json-server db.json --port 3000
```

Le serveur est accessible à l'adresse :

`http://localhost:3000`

Les tickets sont accessibles via :

`http://localhost:3000/tickets`

### Lancement de Vue.js

Dans un deuxième terminal :

```bash
npm run dev
```



## 5. Fonctionnalités réalisées

### Gestion et affichage des tickets

- Récupération des tickets depuis le serveur JSON avec Axios.
- Utilisation de la méthode GET pour récupérer les données.
- Affichage des tickets dans l'interface Vue.js.
- Chargement automatique des tickets avec `onMounted()`.
- Gestion de l'état de chargement avec `ref()`.
- Gestion et affichage des erreurs.

### Recherche et filtrage

- Recherche des tickets par titre.
- Filtrage des tickets par statut.
- Filtrage des tickets par priorité.
- Utilisation de `computed()` pour obtenir automatiquement la liste des tickets filtrés.
- Affichage d'un message lorsqu'aucun ticket ne correspond aux critères de recherche.

## 6. Difficultés rencontrées

- Comprendre le fonctionnement d'Axios et son rôle dans la communication avec une API.
- Configurer Axios avec `axios.create()` et `baseURL`.
- Comprendre les requêtes HTTP et leur fonctionnement.
- Utiliser `ref()` pour gérer les données réactives.
- Comprendre le rôle de `onMounted()` dans le cycle de vie d'un composant Vue.js.
- Utiliser `computed()` pour réaliser la recherche et le filtrage.
- Gérer les erreurs et l'état de chargement des données.

## Questions
## 1-Quelle différence entre une API REST et le fichier db.json?
-db.json est un fichier qui stocke les données en format JSON
-API REST est une interface qui permet de communiquer avec les données à travers des requets HTTP.

## 2-? Pourquoi utiliser onMounted()
-On utilise onMonted pour exécuter une fonction après le montage du composant dans le DOM.

## 3-Quel est le rôle d’Axios
-Axios est une bibliothèque JavaScript qui permet d'envoyer des requêtes HTTP à une API REST pour récupérer, ajouter, modifier ou supprimer des données.

## 4-Quelle différence entre ref() et computed()
-ref() : permet de créer une référence réactive dont la valeur peut être modifiée.
-computed() : permet de créer une valeur calculée qui se met à jour automatiquement lorsque ses dépendances réactives changent.

