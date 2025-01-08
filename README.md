# NewChic Data Analysis: Classification and Clustering
This repository contains the implementation and analysis for CSCI946 Assignment 1, where we explored the NewChic dataset to identify key patterns and classify products based on their performance. The project employs clustering and classification techniques to derive actionable insights.

## Project Overview
The project aimed to address two primary questions:
- Identify the top 10 products across different categories based on their performance.
- Determine the best category among the provided categories.
To achieve these goals, the project incorporated advanced clustering and classification techniques supported by exploratory data analysis and statistical metrics.

## Key Features
**1. Problem Analysis and Preprocessing**
Comprehensive Exploratory Data Analysis (EDA) to understand dataset characteristics and patterns.
Preprocessing steps included:
Handling duplicates.
Normalizing features using StandardScaler.
Addressing multicollinearity using Principal Component Analysis (PCA).
Developed a composite metric combining discounts and customer likes to rank products.
**2. Clustering**
Techniques Used:
KMeans: Identifies well-defined spherical clusters.
Gaussian Mixture Model (GMM): Probabilistic clustering accommodating varied cluster shapes.
DBSCAN: Density-based clustering robust to noise and outliers.
Evaluation Metrics:
Silhouette Score.
Bayesian Information Criterion (BIC).
Elbow Method.
Conducted experiments with and without PCA to understand dataset structure better.
**3. Classification**
Implemented:
Random Forest Classifier: Demonstrated robustness with high recall and F1 scores.
Logistic Regression: Provided interpretable results but struggled with imbalanced classes.
Hyperparameter tuning performed using Optuna.
**4. Results**
Clustering Insights:
KMeans struggled with overlapping clusters, while DBSCAN and GMM offered better-defined clusters.
Classification Outcomes:
Random Forest achieved higher recall (93%) and accuracy (99%) compared to Logistic Regression.
Identified the top-performing categories:
Women and Shoes categories emerged as the best.

## Tools and Libraries
Python: Core programming language.
Scikit-learn: Preprocessing, clustering, and classification.
Optuna: Hyperparameter tuning.
Pandas & NumPy: Data manipulation and analysis.
Matplotlib & Seaborn: Data visualization.

## Key Findings and Recommendations
Findings:
Effective use of PCA improved clustering performance.
Random Forest outperformed Logistic Regression in handling imbalanced datasets

## Recommendations:
Incorporate additional features like time-series data to enhance clustering results.
Address class imbalance with oversampling techniques or cost-sensitive models.
