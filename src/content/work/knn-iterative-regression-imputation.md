---
title: ML Imputations - KNN, Iterative, Regression
publishDate: 2025-02-22 00:00:00
img: /assets/imputation.jpg
img_alt: Iridescent ripples of a bright blue and pink liquid
description: |
  Implemented and compared K-Nearest Neighbors (KNN), regression-based, and iterative imputation techniques to address missing data across multiple real-world datasets. The project evaluates the effectiveness of each method, highlighting their impact on data quality and subsequent machine learning model performance.
tags:
  - Imputation Techniques
  - Machine Learning
  - K-Nearest Neighbors (KNN) 
  - Iterative Imputation
  - Regression Imputation
  - Python
---

This project focuses on addressing the pervasive issue of missing data in datasets, which can significantly hinder the performance of machine learning models. Utilizing Python, the study explores and compares three prominent imputation techniques: K-Nearest Neighbors (KNN) Imputation, Regression Imputation, and Iterative Imputation. Each method is applied to various datasets, including the Adult Census Data, Air Quality Data, and California Housing Data, to assess their efficacy in handling missing values.

**KNN Imputation** involves identifying the 'k' nearest neighbors for a data point with missing values and imputing the missing entries based on the mean or mode of these neighbors. This method is particularly effective when the dataset has a strong correlation between features. However, it can be computationally intensive, especially with large datasets, and may not perform well when the data has high dimensionality or when the missingness is not random.

**Regression Imputation** predicts missing values by leveraging the relationships between variables. By constructing a regression model where the variable with missing data is the dependent variable and other variables serve as independent variables, missing entries can be estimated. While this method can capture linear relationships effectively, it may introduce bias if the underlying assumptions of linearity and homoscedasticity are violated. 

**Iterative Imputation**, inspired by the Multiple Imputation by Chained Equations (MICE) approach, models each feature with missing values as a function of other features in a round-robin fashion. This iterative process continues until convergence, allowing for more accurate and unbiased imputations, especially when dealing with complex datasets with multivariate missing patterns.

The project provides Jupyter notebooks for each dataset, detailing the preprocessing steps, application of each imputation technique, and subsequent evaluation using machine learning models. Performance metrics such as accuracy, mean squared error, and R-squared are used to assess the impact of each imputation method on model performance.

This comprehensive analysis serves as a valuable resource for data scientists and machine learning practitioners, offering insights into the strengths and limitations of various imputation techniques and guiding the selection of appropriate methods based on dataset characteristics.

GitHub Repository: [Imputation Techniques: KNN, Regression, and Iterative Methods](https://github.com/i-archanasenthil/imputation-techniques-knn-regression-iterative)