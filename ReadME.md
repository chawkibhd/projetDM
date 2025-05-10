# Clustering d'Alliages Métalliques via K-Means, ACP et Normalisation

## 📌 Objectif du Projet

Ce projet a pour but de regrouper des alliages métalliques en clusters homogènes selon leur composition chimique, en utilisant des techniques avancées de **prétraitement**, **réduction de dimensionnalité** (ACP), **normalisation**, et **clustering K-Means**.

## 🧪 Données

Les données consistent en des chaînes de composition d’alliages métalliques (ex: `Ag30.8 Ca30.8 Mg23.1 Cu15.4`) nécessitant une décomposition en variables quantitatives exploitables.

## ⚙️ Méthodologie

1. **Prétraitement** :

   * Extraction des éléments chimiques et de leur proportion.
   * Gestion des structures imbriquées complexes.
   * Suppression des colonnes nulles.
   * Remplacement des valeurs manquantes par zéro.

2. **Clustering** :

   * Recherche du meilleur **k** via la méthode du coude (inertie K-Means).
   * Clustering sur les données originales, projetées par ACP, et normalisées.
   * Visualisation des résultats.

3. **Réduction de dimension** :

   * **ACP** utilisée pour une représentation en 2D plus lisible.
   * Application de **StandardScaler** pour homogénéiser les échelles.

## 📈 Résultats

* Le nombre optimal de clusters trouvé est **k = 3**.
* L’ACP améliore nettement la visualisation et la qualité des clusters.
* La normalisation couplée à l’ACP renforce la séparation des groupes.

## 🔍 Perspectives

* Tester des méthodes alternatives : **DBSCAN**, **clustering hiérarchique**.
* Évaluer les résultats avec des métriques comme le **Silhouette Score** ou **Davies-Bouldin Index**.
* Utiliser des techniques non linéaires de réduction de dimension comme **t-SNE** ou **UMAP**.

## 🛠️ Technologies Utilisées

* Python
* Pandas & NumPy
* Scikit-learn (KMeans, PCA, StandardScaler)
* Matplotlib & Seaborn

## 📂 Structure du dépôt

```
📦 project-root/
│
├── data/                               # Raw and processed data
│   ├── row_data.ods                    # Raw, unprocessed files (never modified)
│   ├── cleaned_data.xlsx               # Cleaned or transformed datasets
│   └── cleaned_data_with_cluster.xlsx  # Cleaned or transformed datasets
│
├── notebooks/                          # Jupyter notebooks (exploration, experiments)
│   ├── func_exploration.ipynb
│   └── test_experiments.ipynb
│
├── main.ipynb                          # Source code (scripts and utilities)
│
├── reports/                            # Final reports, PDFs, and documentation
│   ├── Data_Mining_Project_Report.pdf
│
├── docs/                               # Supplementary documents or references
│   └── machine_learning.pdf
│
├── .gitignore
├── requirements.txt
└── README.md                           # Main project readme
```

## 👤 Les Auteurs
- Samir Akram OUNIS
- Chawki BELHADDAD

Les Étudiants en Ingénierie des Systèmes Informatiques Intelligents – Université d’Alger 1
