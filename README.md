# Prédiction des résultats de la Premier League

Ce projet consiste à prédire les résultats des matchs de la **Premier League** en utilisant des **features rolling par équipe** et des **écarts domicile/extérieur**, avec deux modèles de machine learning : **XGBoost** et **RandomForest**.

---

##  Objectif du projet

- Prédire le résultat d’un match :  
  - 0 → Victoire extérieur  
  - 1 → Match nul  
  - 2 → Victoire domicile
- Utiliser des données historiques de **5 saisons (2018-19 à 2022-23)** pour entraîner le modèle
- Évaluer les performances sur des ensembles **train, validation et test** avec un **split temporel** pour éviter la fuite de données

##  Étapes du projet

1. **Data Collection & Preprocessing**  
   - Scraping des données historiques de la Premier League  
   - Nettoyage et renommage des colonnes  
   - Définition de la colonne cible (`cible_resultat`)  

2. **Feature Engineering**  
   - Rolling features par équipe (points, buts, tirs, cartons…)  
   - Calcul des écarts domicile vs extérieur  
   - Visualisation et analyse exploratoire  

3. **Machine Learning**  
   - Split temporel train / val / test  
   - Entraînement de **XGBoost** et **RandomForest**  
   - Évaluation : accuracy, classification report, matrice de confusion  
   - Feature importance pour interprétabilité  
---

## Perspectives / améliorations

- Ajouter plus de features avancées (possession, tirs cadrés, corners…)  
- Hyperparameter tuning (XGBoost et RandomForest)  
- Modèle probabiliste pour prédiction des scores exacts  
- Visualisations interactives des performances par équipe  




