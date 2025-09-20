---
title: "Solveur multigrille appris avec PyTorch"
date: 2025-01-20
categories: [Projets, IA, Numérique]
tags: [Python, PyTorch, Deep Learning, Méthodes numériques, Optimisation]
---

Développement d’un **solveur multigrille appris** pour l’équation de Poisson 2D, en combinant méthodes numériques classiques et apprentissage automatique avec **PyTorch Lightning**.  

### 🎯 Objectif
Explorer différentes stratégies d’optimisation des *smoothers* (opérateurs de relaxation) et des noyaux appris afin d’améliorer la vitesse de convergence par rapport aux solveurs multigrilles traditionnels.  

### 🛠️ Outils & Technologies
- **Python** et **PyTorch Lightning** pour la modélisation et l’entraînement  
- **Visualisation** des noyaux appris, des résidus et de la convergence  
- **Architecture modulaire** avec scripts dédiés : entraînement, inférence, visualisation, checkpoints  

### 📌 Contributions techniques
- Implémentation de plusieurs variantes :  
  - **Level-wise Weighted Jacobi** : poids central appris par niveau  
  - **Fully Adaptive Smoother** : noyau complet appris, avec variantes *par niveau*, *approche généralisée* et *TSK (Transfer Smoothing Kernels)*  
- Mise en place d’une **pipeline complète** : entraînement → inférence → visualisation → sauvegarde  

### 📊 Résultats
- Accélération de la convergence par rapport aux solveurs classiques  
- Analyse graphique et comparaison des performances des différentes variantes  
- Sauvegarde automatisée des modèles et des métriques pour reproductibilité  

### 🔗 Liens
- [Code source GitHub](https://github.com/Saamuel1/stage-multigrille)
