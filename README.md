# 🌌 Astronomical Object Classification Using Machine Learning on SDSS17 Data

> CSC1181 – Foundations of Statistical Analysis & Machine Learning | 2025 Autumn | Dublin City University

## Overview

This project applies machine learning to classify astronomical objects (Stars, Galaxies, Quasars) using the [Stellar Classification Dataset – SDSS17](https://www.kaggle.com/datasets/fedesoriano/stellar-classification-dataset-sdss17) from Kaggle. The dataset contains 100,000 observations with 17 features including photometric filters (u, g, r, i, z) and redshift values.

## Results

| Model | Accuracy | F1 Score |
|---|---|---|
| Logistic Regression (Baseline) | 91.06% | 90.79% |
| Decision Tree | 95.87% | 95.88% |
| Random Forest | 95.87% | 95.88% |
| KNN | 89.78% | 89.49% |
| SVM | 93.13% | 92.97% |
| **Gradient Boosting** | **97.37%** | **97.32%** |
| AdaBoost | 91.53% | 91.76% |
| **XGBoost** | **97.33%** | **97.30%** |

**Best model: Gradient Boosting** with 97.37% accuracy.

Supplementary analysis with improved feature selection further boosted Logistic Regression (+1.0%), Decision Tree (+0.8%), and Random Forest (+2.1%).

## Methods

- **Preprocessing**: Removed unique ID columns, IQR-based outlier removal, MinMax scaling
- **Feature Selection**: Multicollinearity analysis via heatmap; tested multiple feature subsets
- **Validation**: 70/30 train-test split + 5-fold cross-validation
- **Models**: Logistic Regression, Decision Tree, Random Forest, KNN, SVM, Gradient Boosting, AdaBoost, XGBoost

## Repository Structure

```
├── Astronomical_Object_Classification(Codebase).ipynb         # Core models & evaluation
├── Astronomical_Object_Classification(Supplementary).ipynb    # Extended analysis
└── README.md
```

## Dataset

[Stellar Classification Dataset – SDSS17 on Kaggle](https://www.kaggle.com/datasets/fedesoriano/stellar-classification-dataset-sdss17)

## Team

| Name | Student ID | Role |
|---|---|---|
| Varad Abhay Mahadik | A00051764 | Core codebase, data processing, modelling, PPT |
| Shubin Li | A00048674 | Supplementary analysis, error analysis & limitations |
| Aadesh Sunil Kshetre | A00052071 | Code merging, report review, PPT design |
| Yu Yu Lwin | A00053026 | Full report writing & analysis |
