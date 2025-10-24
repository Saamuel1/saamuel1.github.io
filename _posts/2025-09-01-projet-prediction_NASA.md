---
title: "Maintenance Prédictive avec Données Capteurs (NASA CMAPSS)"
date: 2025-09-01
categories: [Projets, IA, Prédiction, Machine Learning]
tags: [LSTM, Random Forest, MAE, Deep Learning]
---
# 

## Objectif
Ce projet avait pour but de démontrer ma capacité à réaliser un cycle complet de data science appliqué à un cas concret d'industrie 4.0.  
L’enjeu n’était pas de battre un benchmark, mais de montrer que je suis capable de :
- Comprendre et préparer des données capteurs complexes.
- Concevoir et évaluer différents modèles de machine learning et deep learning.
- Restituer les résultats sous forme de visualisations claires et exploitables.

## Méthodologie
1. **Préparation des données**
   - Extraction et nettoyage des séries temporelles de capteurs.
   - Construction de la Remaining Useful Life (RUL).
   - Normalisation et création de séquences temporelles pour le deep learning.

2. **Modélisation**
   - **RandomForest baseline** : première approche de référence.
   - **RandomForest avec features avancées** : moyennes et écarts-types glissants.
   - **LSTM amélioré** : capture des dynamiques temporelles pour prédire la RUL.

3. **Évaluation et visualisation**
   - Métriques : RMSE, MAE, R².
   - Visualisations : nuages de points (prédictions vs réalité), suivi individuel des moteurs.
   - Comparaison des performances des modèles.

## Résultats
- **RandomForest baseline** : MAE ≈ 35 cycles.
- **RandomForest amélioré** : stabilité légèrement meilleure.
- **LSTM amélioré** : MAE ≈ 25 cycles, RMSE ≈ 35 → meilleur compromis.

Le modèle LSTM est particulièrement performant pour prédire les pannes proches (RUL faible), ce qui est crucial en maintenance prédictive.

## Compétences démontrées
- Manipulation et transformation de séries temporelles avec **Python (Pandas, NumPy)**.
- Implémentation de modèles ML et DL avec **scikit-learn, TensorFlow/Keras**.
- Visualisation avancée avec **Matplotlib, Seaborn**.
- Mise en place d’une démarche complète de data science : préparation, modélisation, évaluation, restitution.

## Conclusion
Ce projet illustre ma capacité à mener de bout en bout une étude de maintenance prédictive :
- De la donnée brute capteur jusqu’au modèle opérationnel.
- En choisissant et comparant plusieurs approches.
- En mettant l’accent sur la clarté des résultats et leur interprétation

### 🔗 Liens
- [Lien Github](https://github.com/Saamuel1/Projet_Maintenance_predictive)
