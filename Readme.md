# ✈️ Application de Gestion des Voyages 🚀

## Présentation du Projet

Cette application desktop vise à centraliser la gestion des voyages et des clients pour les agences de voyages. Elle est développée en **Java** avec une interface graphique basée sur **Swing**, et suit le modèle **MVC (Modèle-Vue-Contrôleur)** afin d'assurer une séparation claire entre la logique métier, l'interface utilisateur et l'accès aux données. Le projet est développé selon la méthodologie **RUP (Rational Unified Process)**, permettant un développement itératif et incrémental.

---

## Fonctionnalités Implémentées ✅

### Gestion des Clients
- **Ajout, modification, suppression** de clients.
- Affichage et **recherche des clients par CIN** 🔎.
- Utilisation d'une **JTable** pour visualiser la liste des clients.

### Gestion des Voyages
- **Ajout, modification, suppression** de voyages.
- Affichage et **recherche des voyages par destination** 🌍.
- Affichage **dynamique des voyages dans un tableau**.

---

## Fonctionnalités en Cours de Développement 🛠️

### Gestion des Réservations ⚠️🚧
> **Attention :**  
> Le cas d'utilisation concernant la **réservation** n'est **pas encore implémenté**.  
> Il s'agit du dernier cas d'utilisation prévu dans l'étude de domaine, et son développement est en cours.  
> **L'ajout de la fonctionnalité de réservation sera effectué dès que possible.** ⏳🔜

---

## Structure du Projet 📂

L'application est organisée en plusieurs packages pour assurer une architecture modulable et maintenable :

- **IHM**  
  Contient les classes d'interface utilisateur (Swing) telles que `GestionClientIHM` et `GestionVoyagesIHM`.

- **entity**  
  Définit les entités du domaine : `Client`, `Voyage`.

- **controller**  
  Regroupe les contrôleurs qui font le lien entre l'interface et l'accès aux données, par exemple `ClientController` et `VoyageController`.

- **dao**  
  Contient les classes d'accès aux données (DAO) pour effectuer les opérations CRUD sur la base de données, telles que `ClientDAO` et `VoyageDAO`.

- **db**  
  Contient la logique de connexion à la base de données via JDBC.

---

## Méthodologie Utilisée 📈

Le projet est développé selon le **Rational Unified Process (RUP)** :

- **Inception**  
  Définition de la vision, recueil des besoins, et établissement des premiers cas d'utilisation.

- **Elaboration**  
  Analyse fonctionnelle détaillée, définition de l'architecture (ex. utilisation du modèle MVC et des design patterns comme le Singleton).

- **Construction**  
  Développement des fonctionnalités existantes (Gestion des Clients et Voyages) avec intégration de tests unitaires et fonctionnels.

- **Transition**  
  Déploiement progressif prévu avec des itérations sur les retours utilisateurs.

> **Note Importante 🚨 :**  
> Le module de **Réservations** est le dernier cas d'utilisation prévu et sera implémenté dans une prochaine version du projet.

---

## Installation et Exécution 💻

### Prérequis
- **Java SE** (version 8 ou supérieure)
- Un **IDE** compatible (par exemple, **NetBeans** ou **Eclipse**)
- Une base de données (configuration JDBC à adapter dans la classe de gestion de connexion, généralement présente dans le package **db**)

### Compilation et Exécution
1. **Cloner** le dépôt GitHub sur votre machine.
2. **Ouvrir** le projet dans votre IDE favori.
3. **Configurer** la connexion à la base de données.
4. **Compiler** et **exécuter** la classe principale de votre module, par exemple `GestionClientIHM.java` ou `GestionVoyagesIHM.java`.

---

## Utilisation 🖥️

### Gestion Clients
- Utilisez l'IHM dédiée pour **ajouter, modifier, supprimer** et **rechercher des clients**.  
- La recherche se fait par **CIN**, et le tableau se rafraîchit automatiquement après chaque opération.

### Gestion Voyages
- De manière similaire, l'IHM **Gestion Voyages** permet d'**ajouter, modifier, supprimer** des voyages et de **rechercher par destination**.


---


## Tests et Qualité du Code 🧪🔍

Ce projet intègre une série de tests unitaires afin de garantir la robustesse et la fiabilité des fonctionnalités développées. Parmi les outils utilisés, nous avons :

- **JUnit**  
  Des tests unitaires ont été réalisés sur les composants clés de l’application :
  - **ClientControllerTest** : Vérifie les opérations d’ajout, modification, suppression, consultation et recherche des clients.
  - **VoyageControllerTest** : Assure le bon fonctionnement des méthodes d’ajout, modification, suppression et recherche des voyages.
  - **Tests des entités et DAO** (ClientTest, ClientDAOTest, VoyageTest) : Valident la cohérence des constructeurs, getters/setters, les méthodes de transformation (toArray, toString) et les interactions avec la base de données.

- **JaCoCo**  
  Cet outil est utilisé pour mesurer la couverture de tests du projet, garantissant que la majorité des classes et méthodes critiques sont couvertes par des tests automatiques. Cela contribue à détecter rapidement les régressions et à améliorer la maintenabilité du code.

Ces tests sont essentiels pour maintenir la qualité du code et pour faciliter l’évolution de l’application dans le cadre de la méthodologie RUP (Rational Unified Process).



---

## Projets Futurs et Améliorations 🔮

- **Implémentation de la Gestion des Réservations**  
  Le module des **réservations** sera ajouté dans un futur proche pour compléter l'application.
  
- **Optimisation et Tests**  
  Poursuite des tests unitaires et d'intégration pour garantir la robustesse de l’application.

---

## Contribuer 🤝

Les contributions sont les bienvenues !  
Si vous souhaitez apporter des améliorations ou proposer des corrections, n'hésitez pas à forker le dépôt et à soumettre des Pull Requests.

