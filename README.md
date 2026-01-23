# 📊 Bank Customer Data Analysis & Churn Prediction (Python)

## 📌 Project Overview

This project combines an **exploratory data analysis (EDA)** and a **personal predictive modeling extension by Javier Gonzálvez** based on a real-world banking customer dataset.

The **EDA and data preprocessing** were originally developed as a **group academic project** for the course **Programming I** during the **first year of the Degree in Mathematical Engineering**.

Building upon that foundation, the project was **individually extended as a personal project** with the objective of transitioning from descriptive analysis to a **simple and interpretable predictive model** focused on **customer churn**.

The overall goal of the project is to:
- Understand customer behavior through data exploration
- Apply rigorous data cleaning and preprocessing
- Formulate a realistic classification problem
- Train, evaluate, and interpret a basic machine learning model aligned with business objectives

---

## 🧑‍💻 Authors

### Academic EDA (Group Work)
- **Jairo Sánchez Díaz-Concha**
- Javier Gonzálvez Sempere
- Luis González Gómez

### Predictive Modeling Extension
- Javier Gonzálvez Sempere (individual work)

---

## 🗂 Dataset

- **Source:** Kaggle (public dataset)
- **Size:** 10,127 customers × 23 variables
- **Content:**  
  Demographic, financial, and behavioral information related to bank customers and credit card usage.

> ⚠️ The original CSV file may not be included in this repository due to licensing or sharing restrictions.  
> Dataset available at:  
> https://www.kaggle.com/datasets/sakshigoyal7/credit-card-customers

---

## 🛠 Tools & Technologies

- Python
- pandas
- numpy
- matplotlib
- scikit-learn

---

## ▶️ How to Run

1. Clone the repository
2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib scikit-learn
Open the Jupyter notebook and run all cells sequentially.

🔧 Data Preprocessing
The dataset required several preprocessing steps to ensure consistency and statistical validity:

Initial data inspection (shape, data types, missing values)

Detection and treatment of outliers

Custom statistical imputation strategy:

Median for skewed distributions

Mean for approximately symmetric distributions

Conversion of categorical income ranges into numerical values

Renaming columns for clarity and maintainability

Removal of irrelevant or redundant variables

📈 Exploratory Data Analysis (EDA)
The exploratory analysis includes:

Descriptive statistics using custom-built functions

Visualization of distributions (histograms and boxplots)

Identification of outliers and anomalous patterns

Correlation analysis between numerical variables

Visual exploration of linear and non-linear relationships

🔍 Key Findings from EDA
Variable redundancy:
A strong linear relationship between Credit Limit and Average Open to Buy suggests redundancy and potential multicollinearity.

Customer activity patterns:
Transaction count and transaction amount clearly differentiate customer behavior profiles.

Financial risk indicators:
Higher utilization ratios combined with lower credit limits may indicate early financial stress.

Feature engineering:
Simple risk indicators related to inactivity and usage were derived to support further analysis.

🤖 Predictive Modeling: Customer Churn (Personal Extension)
Based on the exploratory findings, the project was extended into a binary classification problem aimed at predicting customer churn.

The target variable represents:

0 → Active customer

1 → Customer who has abandoned the bank

A logistic regression model was selected due to its:

Interpretability

Suitability for binary outcomes

Direct link between coefficients and customer behavior

Main steps:

Binary encoding of the target variable

Train–test split preserving class proportions

Feature scaling via standardization

Baseline model training and evaluation

📊 Model Evaluation & Improvement
The initial model achieved good overall accuracy but showed limited recall for the churn class.

Since detecting customers at risk of leaving is more relevant than minimizing false positives, several improvements were applied:

Class balancing

Adjustment of the decision threshold

Analysis of the trade-off between precision and recall

These changes resulted in a model better aligned with business objectives.

🔎 Model Interpretation
The final model coefficients were analyzed to assess feature importance:

Variables related to customer activity (e.g. transaction count and inactivity months) have the strongest influence.

Higher engagement is associated with a lower probability of churn.

Reduced usage and prolonged inactivity significantly increase churn risk.

These results are consistent with the patterns observed during the EDA phase.

🎓 What I Learned
Through this project, I gained experience in:

Working with real-world datasets

Applying statistical reasoning to preprocessing decisions

Designing a complete data analysis workflow

Transitioning from EDA to predictive modeling

Interpreting models in a business context

Understanding metric trade-offs

📎 Notes
The EDA corresponds to an academic group assignment

The predictive modeling section is a personal project extension

The focus is on clarity, reasoning, and interpretability

🇪🇸 Resumen en español
Proyecto de análisis de datos de clientes bancarios con Python.
Incluye un análisis exploratorio realizado en grupo y una extensión individual de modelado predictivo para anticipar el abandono de clientes mediante regresión logística.
Se prioriza la interpretación y el razonamiento frente a la complejidad del modelo.


    Análisis de datos de clientes de un banco  © 2025 by Jairo Sánchez Díaz-Concha, Javier Gonzálvez Sempere y Luis González Gómez is licensed under Creative Commons Attribution-NonCommercial 4.0 International. To view a copy of this license, visit https://creativecommons.org/licenses/by-nc/4.0/
