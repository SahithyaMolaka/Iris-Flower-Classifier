# Iris-Flower-Classifier
Multi-model ML project for classifying Iris flowers

## Project Overview
The **Iris Flower Classifier** predicts the species of an Iris flower (`Setosa`, `Versicolor`, `Virginica`) based on four features:  
**sepal length, sepal width, petal length, and petal width**.  

This project implements **multiple machine learning models**, compares their performance, and demonstrates an end-to-end machine learning workflow from data exploration to model evaluation and optional deployment.

**Skills Demonstrated:**  
- Data exploration and visualization (EDA)  
- Multi-class classification  
- Model comparison and evaluation  
- Feature importance analysis  
- Optional deployment with Streamlit  

---

## Dataset
- **Source:** [UCI Iris Dataset](https://archive.ics.uci.edu/ml/datasets/iris)  
- **Samples:** 150  
- **Features:** 4 numeric features  
- **Target:** Species (`Setosa`, `Versicolor`, `Virginica`)  
- **Description:** Each row represents one flower with measurements of sepal length/width and petal length/width.  

---

## Exploratory Data Analysis (EDA)
- Pairplots and boxplots show that **petal length and width clearly separate species**, especially `Setosa`.  
- Sepal features overlap more between `Versicolor` and `Virginica`.  
- Dataset is clean, with **no missing values** and **balanced classes**.  

---

## Models Implemented

| Model | Type | Notes |
|-------|------|-------|
| Logistic Regression | Linear classifier | Baseline model |
| K-Nearest Neighbors (KNN) | Instance-based | Sensitive to feature scaling |
| Decision Tree | Tree-based | Captures non-linear patterns |
| Random Forest | Ensemble of trees | Reduces overfitting |
| Support Vector Machine (SVM) | Linear/Non-linear | Works well with scaled features |
| Naive Bayes | Probabilistic | Assumes feature independence |

---

## Model Evaluation

**Metrics Used:** Accuracy, Confusion Matrix, Precision, Recall, F1-Score  

**Random Forest Performance Example:**

| Species | Precision | Recall | F1-Score |
|---------|----------|--------|----------|
| Setosa | 1.00 | 1.00 | 1.00 |
| Versicolor | 1.00 | 0.92 | 0.96 |
| Virginica | 0.92 | 1.00 | 0.96 |

**Model Accuracy Comparison:**

| Model | Accuracy |
|-------|---------|
| Random Forest | 97–100% |
| Decision Tree | 93–97% |
| KNN | 96% |
| Logistic Regression | 95% |
| SVM | 97% |
| Naive Bayes | 94% |

---

## Feature Importance (Random Forest)
- **Petal length & width** are the most important features for classification.  
- **Sepal features** contribute less but still aid in prediction.

---

## Optional Deployment
- A **Streamlit app** allows users to input flower measurements and get **real-time species predictions**.  

---

## Key Learnings
- Multi-class classification can be effectively handled with simple models.  
- Tree-based ensembles like Random Forest outperform single models in robustness.  
- Feature scaling is critical for distance-based algorithms like KNN and SVM.  
- Visualizations help identify predictive features and understand dataset patterns.  

---

## Extensions & Improvements
- Apply **PCA/t-SNE** for dimensionality reduction and visualization.  
- Hyperparameter tuning using **GridSearchCV** for better performance.  
- Add **SHAP values** for explainable predictions.  
- Deploy a web app for **interactive user input**.  

---

## Tools & Libraries
- **Python 3.x**  
- Libraries: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`, `streamlit`  

---


