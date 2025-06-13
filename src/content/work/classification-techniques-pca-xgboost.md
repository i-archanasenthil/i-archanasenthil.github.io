---
title: Wine Classification - PCA, XGBoost
publishDate: 2025-02-25 00:00:00
img: /assets/wine.jpg
img_alt: A chatbot in a blue background
description: |
  Developed a machine learning pipeline to classify wine types based on physicochemical properties, utilizing XGBoost for classification and Principal Component Analysis (PCA) for dimensionality reduction. The project includes data preprocessing, model training, evaluation, and visualization of results.
tags:
  - Python 
  - Classification Model
  - PCA Principal Component Analysis
  - XGBoost Extreme Gradient Boosting
  - BayesSearchCV
---

This project explores the application of machine learning for classifying wines based on their chemical attributes. Using a publicly available dataset from the UCI Machine Learning Repository, it includes both red and white wine samples with 13 physicochemical properties. The objective was to accurately differentiate wine types using a predictive model that is both high-performing and interpretable. The workflow integrates preprocessing, feature reduction through Principal Component Analysis (PCA), model training using XGBoost, and performance tuning through Bayesian Optimization. Each stage contributes to building a robust classification pipeline and reveals the most influential features in wine characterization.

**Data Preprocessing**

The dataset was first prepared by combining red and white wine data and performing standard cleaning steps such as removing missing values and encoding target labels. To ensure consistency, numerical features like fixed acidity, citric acid, and alcohol content were standardized. This preprocessing was crucial to ensure that all features were on a similar scale, especially important before applying PCA and training gradient boosting models. The class labels were encoded into binary format to support supervised classification.

**Dimensionality Reduction with PCA**

Principal Component Analysis (PCA) was used to reduce the dimensionality of the dataset while retaining the majority of its variance. By projecting the high-dimensional data into a lower-dimensional space, PCA facilitated better visualization and reduced computational overhead. Visual analysis of the first two principal components showed a degree of separation between wine classes, validating the effectiveness of PCA for exploratory analysis and feature compression.

**Model Development with XGBoost**

The classification model was developed using XGBoost, a scalable and high-performance gradient boosting framework known for its regularization capabilities and handling of structured data. XGBoost was chosen for its speed, flexibility, and ability to capture non-linear relationships. It also provides inherent support for feature importance, which was later used for interpretability. The model was trained on the full feature set and later re-evaluated after dimensionality reduction, with consistent performance across both.

**Hyperparameter Tuning with BayesSearchCV**

To optimize model performance, Bayesian hyperparameter optimization was implemented using BayesSearchCV from the scikit-optimize package. This technique uses probabilistic modeling to intelligently explore the hyperparameter space, offering a more efficient alternative to grid or random search. Key parameters such as learning rate, maximum tree depth, number of estimators, and subsample ratios were tuned. This process improved model generalization and reduced overfitting by fine-tuning the learning process based on past evaluation results.

**Model Evaluation and Visualization**

Model performance was evaluated using standard classification metrics such as accuracy, and the area under the ROC curve (AUC). Confusion matrices were plotted to identify classification errors and class imbalances. In addition, feature importance scores from XGBoost were visualized to highlight the most influential predictors—alcohol content, volatile acidity, and citric acid emerged as key features in distinguishing wine types. PCA scatter plot further illustrated the separation between classes and helped validate the model's assumptions and decisions.

This end-to-end machine learning solution demonstrates how a combination of data-driven modeling, dimensionality reduction, and advanced optimization techniques can be applied effectively in the food and beverage domain. It also shows how interpretability and performance can go hand-in-hand when careful consideration is given to each stage of the pipeline.

🔗 GitHub Repository: [Wine Classification Analysis](https://github.com/i-archanasenthil/wine-classification-analysis)
