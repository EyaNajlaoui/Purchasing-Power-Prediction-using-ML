# Purchasing Power Prediction using Machine Learning

## 📌 Project Overview
This project was developed as part of an academic course in **Financial Modeling**. The goal is to build a machine learning model that accurately predicts **purchasing power** based on a comprehensive set of economic and financial indicators. The project demonstrates a complete data science workflow—from data preprocessing and exploratory analysis to model training, optimization with `RandomizedSearchCV`, evaluation, and advanced interpretability using SHAP analysis.

## 🎯 Objectives
- To predict purchasing power using regression models
- To compare the performance of **Linear Regression**, **Random Forest**, and **XGBoost**
- To optimize models using **RandomizedSearchCV** for hyperparameter tuning
- To perform **advanced model interpretability** using SHAP (SHapley Additive exPlanations)
- To identify key economic drivers and their directional impact on purchasing power

## 📊 Dataset
The dataset contains **19 key economic and financial indicators** such as:
- **Commodity Prices**
- **Economic Indicators**
- **Income and Consumption Metrics**
- **Financial Market Indices**

## 🛠️ Methodology
### 1. **Data Preprocessing**
- Handling missing values
- Feature scaling (StandardScaler)
- Train-test split (80% train, 20% test)

### 2. **Models Implemented**
- **Linear Regression** (baseline)
- **Random Forest Regressor**
- **XGBoost Regressor**

### 3. **Model Optimization**
- Hyperparameter tuning using **`RandomizedSearchCV`** for efficient optimization
- Evaluation metrics: **Mean Squared Error (MSE)**, **Root Mean Squared Error (RMSE)**, **R² Score**

### 4. **Advanced Model Interpretability**
- **SHAP analysis** for global and local interpretability
- Feature importance quantification with directional impact analysis
- **Individual prediction breakdown** for specific observations
- Visualization of positive/negative contributions per feature

## 📈 Results

### **Model Performance Comparison**
After evaluating all three models with hyperparameter optimization via `RandomizedSearchCV`, the **Random Forest Regressor** demonstrated the best overall performance, achieving an optimal balance between training accuracy and generalization capability.

| Model               | Training MSE | Training R² | Test MSE  | Test R²    |
|---------------------|--------------|-------------|-----------|------------|
| **Random Forest**   | **0.037936** | **0.987249**| **0.143307**| **0.912596** |
| Linear Regression   | 0.272839     | 0.908294    | 0.198808  | 0.878746   |
| XGBoost             | 0.052491     | 0.982357    | 0.208221  | 0.873005   |

