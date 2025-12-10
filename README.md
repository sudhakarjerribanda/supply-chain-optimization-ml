# Predictive Maintenance for Supply Chain Resilience Using Machine Learning

This project applies machine learning to improve E-commerce supply chain efficiency by predicting late deliveries, analysing demand patterns, and identifying operational risks. The dataset used is the DataCo Supply Chain dataset, which contains customer, product, shipping, and transactional information.

The goal of this project is to reduce delivery delays, enhance forecasting accuracy, improve planning decisions, and increase overall supply chain resilience.

---

## Project Objectives

- Identify factors that contribute to late deliveries.
- Perform exploratory data analysis (EDA) to understand dataset patterns.
- Build and compare multiple machine learning models.
- Use feature engineering to improve prediction accuracy.
- Evaluate performance using accuracy, precision, recall, and F1 score.
- Provide insights to support better supply chain decision-making.

---

## Dataset Description

The dataset contains:

- 180,519 rows  
- 53 features  
- Product categories: Clothing, Sports, Electronics  
- Target variable: `late_delivery` (binary classification)

Dataset attributes include customer demographics, order quantities, pricing, shipment modes, product details, and timestamps.

---

## Data Preprocessing

Key preprocessing steps include:

- Handling missing values
- Removing outliers
- One-hot encoding of categorical variables
- Feature scaling using StandardScaler
- Train-test split (70% training, 30% testing)
- Feature engineering using known formulas:
  - Sales = Product Price × Quantity  
  - Order Item Total = Sales − Discount  

---

## Exploratory Data Analysis Summary

Important findings:

- Around 55% of orders experienced late delivery.
- Europe generated the highest profit per order; LATAM generated the highest order volume.
- Second-Class shipping mode had the highest late-delivery rate.
- Higher product prices generally resulted in lower quantities ordered.
- Several features showed strong correlations affecting delivery performance.

---

## Machine Learning Models Implemented

The following classification models were used:

- Random Forest Classifier  
- Support Vector Machine (SVM)  
- Logistic Regression  
- Linear Discriminant Analysis (LDA)  
- Gaussian Naive Bayes  

Evaluation metrics: Accuracy, Precision, Recall, F1 Score.

Random Forest produced the best results with an F1 Score of 99.49%.

---

## Model Evaluation Summary

| Model                       | Accuracy  | F1 Score | Notes                             |
|-----------------------------|-----------|----------|-----------------------------------|
| Random Forest               | 99.44%    | 99.49%   | Best performing model             |
| Support Vector Machine      | 98.25%    | 98.44%   | Strong overall performance        |
| Logistic Regression         | 98.24%    | 98.43%   | Reliable baseline                 |
| Linear Discriminant Analysis| 96.20%    | Lower    | Misses some late deliveries       |
| Gaussian Naive Bayes        | 94.58%    | 95.29%   | Least effective model here        |

---

## Tools and Technologies

- Python
- Jupyter Notebook
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Statsmodels (OLS Regression)

---

## Project Workflow

1. Data Cleaning and Preprocessing  
2. Exploratory Data Analysis  
3. Feature Engineering  
4. Model Training  
5. Model Evaluation  
6. Insights and Conclusions  

---

## Recommended Folder Structure

