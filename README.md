# FIRE Tracker Pro - Ultimate Edition 🚀📊

FIRE Tracker Pro est une application web tout-en-un sous la forme d'un tableau de bord interactif. Elle est conçue pour aider les utilisateurs à planifier leur indépendance financière (FIRE - Financial Independence, Retire Early), suivre leurs flux de trésorerie (Cash Flow), et simuler la croissance de leur patrimoine via les intérêts composés.

## ✨ Fonctionnalités Principales

L'application est divisée en trois modules distincts, accessibles via la barre de navigation supérieure :

### 1. 🚀 Simulateur FIRE
Un module prédictif pour calculer l'âge de votre retraite ou l'effort d'épargne nécessaire.
* **Calcul Bidirectionnel :** Calculez l'âge de votre retraite en fonction de votre épargne, ou l'épargne requise pour partir à un âge précis.
* **Horloge Macro-économique :** Une boussole interactive permettant d'ajuster l'inflation et la croissance du PIB pour simuler différents climats économiques (Surchauffe, Stagflation, Reflation, Recovery). Les données peuvent être extraites automatiquement via l'API de la Banque Mondiale.
* **Scénarios Multiples :** Affichage simultané des projections Pessimistes, Neutres et Optimistes sur un graphique linéaire dynamique.
* **Jalons FIRE :** Suivi en temps réel de votre progression vers le *Coast FIRE* (50%) et le *FIRE* (100%).

### 2. 📊 Menu Cash Flow
Un gestionnaire de budget pour cartographier vos revenus et vos dépenses.
* **Saisie intuitive :** Ajoutez des entrées et sorties d'argent avec des montants, des titres et des icônes personnalisées.
* **Diagramme de Sankey :** Visualisation avancée des flux financiers de la source (revenus) vers la destination (dépenses et épargne).
* **Graphiques Comparatifs :** Vue en colonnes pour comparer les entrées et sorties.
* **Graphiques de Répartition :** Diagrammes circulaires (Doughnut charts) pour analyser précisément la part de chaque dépense ou revenu.
* **Synchronisation FIRE :** La capacité d'épargne nette calculée est automatiquement synchronisée avec le simulateur FIRE.

### 3. 📈 Intérêts Composés
Un simulateur dédié pour visualiser la croissance de votre capital sur le long terme.
* **Paramètres précis :** Ajustement du capital initial, de l'épargne mensuelle, de l'horizon de placement (années) et du taux d'intérêt.
* **Fréquence de capitalisation :** Possibilité de basculer entre une capitalisation Mensuelle et Annuelle.
* **Graphique en Aires Empilées :** Distinction visuelle claire entre le capital investi (les versements) et les gains générés (les intérêts).

## 🛠️ Technologies Utilisées

Le projet est construit entièrement côté client (Front-end), sans nécessité de serveur ou de base de données externe. Il utilise le LocalStorage du navigateur pour sauvegarder vos flux de trésorerie.

* **HTML5 / CSS3 / JavaScript (ES6)** : Les fondations de l'application.
* **Tailwind CSS** : Framework utilitaire injecté via CDN pour un design moderne, *glassmorphism* et 100% *responsive* (mobile-friendly).
* **Chart.js** : Librairie de datavisualisation pour les graphiques linéaires, en barres et circulaires.
* **Google Charts** : Utilisé spécifiquement pour le rendu complexe du diagramme de flux de trésorerie (Sankey Diagram).

## 💻 Installation et Utilisation

L'application est "Zero-Install". 

1. Téléchargez ou clonez le dépôt.
2. Assurez-vous d'avoir une connexion internet active (nécessaire pour charger Tailwind, Chart.js et Google Charts via leurs CDN respectifs).
3. Ouvrez simplement le fichier `index.html` dans n'importe quel navigateur web moderne (Chrome, Firefox, Safari, Edge).

## 📱 Compatibilité Mobile

L'interface a été méticuleusement pensée pour les petits écrans :
* La barre de navigation s'adapte en colonne ou avec un défilement horizontal.
* Les graphiques ont été corrigés avec des hacks CSS (notamment `overflow-x: auto` pour le diagramme Sankey) pour garantir une lisibilité parfaite même sous les résolutions inférieures à 320px.
* L'ordre des éléments s'inverse sur mobile (affichage du graphique avant les cartes de scores) pour privilégier l'expérience utilisateur.

## 📝 Avertissement

*Les calculs fournis par cet outil sont des estimations basées sur des modèles mathématiques théoriques à taux constants. Ils ne constituent en aucun cas des conseils financiers personnalisés. Les performances passées des marchés ne préjugent pas de leurs performances futures.*
