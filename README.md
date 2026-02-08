# 🚀 GraphOptim-France : Suite d'Optimisation de Réseaux

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)
![NetworkX](https://img.shields.io/badge/NetworkX-61DAFB?style=for-the-badge&logo=networkx&logoColor=black)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)

**GraphOptim-France** est une application interactive de Théorie des Graphes permettant de visualiser et d'appliquer les algorithmes les plus célèbres du domaine sur un réseau routier français réel ainsi que sur des problématiques d'ordonnancement industriel.

---

## 🌟 Fonctionnalités Clés

L'application intègre une suite complète d'outils d'analyse et d'optimisation :

* **Exploration Topologique :** Parcours en largeur (**BFS**) et en profondeur (**DFS**) pour l'analyse de connexité.
* **Optimisation d'Infrastructure :** Calcul de l'Arbre Couvrant Minimum (**ACPM**) via les algorithmes de **Prim** et **Kruskal**.
* **Calcul d'Itinéraires (PCC) :** * **Dijkstra** pour l'efficacité sur réseaux à poids positifs.
    * **Bellman-Ford** pour la gestion des poids négatifs et la détection de cycles.
    * **Floyd-Warshall** pour une analyse matricielle globale et calcul de centralité.
* **Analyse de Flux :** Détermination du débit maximum entre pôles urbains avec **Ford-Fulkerson**.
* **Gestion de Projet (PERT) :** Modélisation de tâches, calcul du **chemin critique** et génération dynamique de **diagrammes de Gantt** interactifs.
* **Interface GUI Moderne :** Un tableau de bord interactif piloté par `ipywidgets` pour une démonstration en temps réel.

---

## 🛠️ Installation et Démarrage Rapide

Le projet est conçu pour être exécuté sans configuration lourde directement dans un environnement Jupyter.

### 1. Prérequis
Assurez-vous d'avoir Python installé ainsi que les bibliothèques suivantes :
```bash
pip install networkx matplotlib pandas ipywidgets numpy
```
2. Lancement

    Téléchargez ou clonez ce dépôt GitHub.

    Ouvrez le fichier .ipynb dans Jupyter Notebook, JupyterLab ou Google Colab.

    Utilisez la commande "Run All Cells" (Exécuter tout).

    L'interface de contrôle apparaîtra automatiquement à la fin du notebook.

🖥️ Aperçu de l'Interface

L'interface utilisateur permet de basculer dynamiquement entre les algorithmes, de choisir les villes de départ et d'arrivée, et d'observer instantanément les résultats graphiques et textuels.

    Exemple : Visualisation d'un plus court chemin calculé via Dijkstra entre Rennes et Marseille.

🏗️ Architecture du Code

Le projet adopte une structure modulaire et pédagogique :

    Moteurs Algorithmiques : Chaque cellule contient l'implémentation brute d'un algorithme (logique pure). L'utilisateur peut consulter le code source pour analyser les choix de structures de données.

    Moteur de Rendu : Fonctions de dessin optimisées pour éviter les superpositions et garantir la lisibilité des poids et chemins.

    Couche d'Abstraction GUI : La dernière cellule centralise tous les modules dans une interface ipywidgets, assurant une séparation claire entre le calcul et l'affichage.

Projet réalisé dans le cadre de l'unité ALMF51 - Analyse et Optimisation de Réseaux (Promotion 2025-2026).
