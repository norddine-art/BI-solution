# Développement d’un Tableau de Bord Commercial - Projet de Stage

[cite_start]Ce dépôt contient le projet réalisé dans le cadre de mon stage d'initiation [cite: 1] [cite_start]au sein de la société **COPAG**[cite: 8]. L'objectif principal était la conception et la mise en œuvre d'une solution de Business Intelligence pour le suivi et l'analyse des performances commerciales.

##  contexte du projet

* [cite_start]**Entreprise d'accueil :** COPAG [cite: 8]
* [cite_start]**Établissement :** École Supérieure de Technologie Essaouira (ESTE) [cite: 2]
* [cite_start]**Auteur :** Abahous Nor-eddine [cite: 6]
* [cite_start]**Encadrant pédagogique :** Mr. Ait Ouakrim Abdessamad [cite: 7]
* [cite_start]**Année Universitaire :** 2025-2026 [cite: 5]

## 🎯 Objectif de la mission

[cite_start]L'objectif était de développer un tableau de bord commercial [cite: 9] permettant aux décideurs de visualiser et d'analyser les indicateurs clés de performance (KPIs) liés aux ventes.

[cite_start]La solution couvre l'ensemble de la chaîne décisionnelle : de l'extraction des données brutes jusqu'à la visualisation interactive[cite: 30, 31].

## 🛠️ Architecture de la Solution

[cite_start]Le projet suit une architecture décisionnelle classique[cite: 30, 31]:

1.  **Sources de Données :** Données opérationnelles et externes de l'entreprise.
2.  [cite_start]**ETL (SSIS) :** Extraction des données et chargement dans un **Data Lake**[cite: 30, 35].
3.  [cite_start]**ETL (SSIS) :** Transformation des données brutes du Data Lake et chargement dans un **Data Warehouse (DWH)** [cite: 30, 38][cite_start], modélisé en schéma en étoile/flocon (MCD)[cite: 22].
4.  [cite_start]**Cube OLAP (SSAS) :** Création d'un modèle tabulaire (Cube) [cite: 40] [cite_start]par-dessus le DWH pour optimiser les performances d'analyse et définir les mesures métier en DAX[cite: 41].
5.  [cite_start]**Restitution (Power BI) :** Connexion au Cube SSAS pour la création du **tableau de bord** interactif[cite: 30, 43].

## 💻 Outils et Technologies

[cite_start]Voici les principaux outils utilisés pour la réalisation de ce projet[cite: 24, 25]:

* [cite_start]**SGBD :** SQL Server (pour le Data Lake et le Data Warehouse [cite: 32])
* [cite_start]**ETL :** Microsoft Visual Studio avec SQL Server Integration Services (SSIS) [cite: 25]
* [cite_start]**Cube (Modélisation) :** SQL Server Analysis Services (SSAS) [cite: 25]
* [cite_start]**Langage de mesure :** DAX (Data Analysis Expressions) [cite: 25]
* [cite_start]**Data Visualisation :** Power BI [cite: 25]

## 📂 Contenu du Dépôt

Ce dépôt est structuré comme suit :

* `/presentation/`: Contient la présentation PowerPoint du stage (`présentation de stage d'initiation.pptx`).
* `/scripts_sql/`: (À AJOUTER) Vous pouvez placer ici vos scripts de création de tables, de vues ou de procédures stockées.
* `/packages_ssis/`: (À AJOUTER) Vous pouvez placer ici vos fichiers de projet et packages SSIS (.dtsx).
* `/modele_ssas/`: (À AJOUTER) Vous pouvez placer ici les fichiers de votre projet de modèle tabulaire SSAS.
* `/rapport_powerbi/`: (À AJOUTER) Vous pouvez placer ici votre fichier final `.pbix`.
* `README.md`: Ce fichier.

---
