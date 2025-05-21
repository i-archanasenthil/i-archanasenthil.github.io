---
title: AF Risk Prediction
publishDate: 2025-02-25 00:00:00
img: /assets/hospital-heart.jpg
img_alt: A heart with an arrow
description: |
  Developed a web application that assesses the risk of Atrial Fibrillation using ECG signals and electronic health records. Integrated data processing, risk prediction models, and a user-friendly interface for clinical insights
tags:
  - Python
  - XGBoost 
  - BayesSearchCV
  - User Interface
  - Chatbot Implementation
  - Health data Analysis and Modeling
  - Interactive dashboard using Dash
---

This project focuses on predicting the risk of new-onset Atrial Fibrillation (AF) by integrating 12-lead ECG signal data with electronic health records (EHR). A robust machine learning pipeline was developed to analyze clinical and signal-derived features, leveraging the power of the XGBoost classifier to produce accurate and interpretable risk scores for AF. The ECG features combined with EHR data such as age, blood pressure, and comorbidities were used to build a comprehensive dataset.

To support model transparency and clinical interpretability, SHAP (SHapley Additive exPlanations) values were used to identify and visualize the contribution of each feature to the model's predictions. This enabled both clinicians and users to understand which health indicators most strongly influenced a patient’s AF risk, aligning with the principles of explainable AI in healthcare.

Exploratory Data Analysis (EDA) was performed using Dash, a Python framework for building interactive web-based dashboards. This component allowed for dynamic visualization of patient demographics, comorbidity distributions, ECG-derived metrics, and correlations between variables—facilitating deeper insights into the data before modeling.

The complete solution was deployed as an interactive web application using Streamlit. The app allows users to input health parameters and receive real-time AF risk predictions, accompanied by a SHAP-based breakdown of the most influential factors. This end-to-end tool combines clinical relevance, machine learning rigor, and user-friendly design, and is intended to assist healthcare providers and researchers in early identification and preventive care for atrial fibrillation.

Also, the chatbot was built on top of the DeepSeek framework and has been customized to analyze and summarize patient information in a clinically meaningful way. It is designed not only to interpret distributions of key health indicators but also to extract relevant insights from patient data. Additionally, it is programmed to provide clear, contextual explanations and, when appropriate, offer preliminary recommendations or flag areas for further clinical review, making it a valuable tool for both data exploration and patient-specific interpretation.

You can explore the deployed application here: [Atrial Fibrillation Risk Prediction App](https://atrialfibrillation-riskpred.streamlit.app/)
GitHub Repository: [AF Risk Pred](https://github.com/i-archanasenthil/af_risk_prediction_using_ecg_and_ehr_data)
