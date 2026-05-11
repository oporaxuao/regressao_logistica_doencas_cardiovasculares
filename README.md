# 🫀 Cardiovascular Disease Prediction with Logistic Regression

Binary classification model to predict cardiovascular disease risk based on clinical data and lifestyle habits, built as a baseline for clinical decision support.

---

## 🎯 Business Objective

Cardiovascular disease is one of the leading causes of death worldwide. Early detection based on routinely collected clinical data can dramatically improve patient outcomes. This project builds a predictive model that estimates a patient's probability of having cardiovascular disease using variables such as age, weight, glucose levels, alcohol consumption, and physical activity — enabling preventive screening at scale.

---

## 🗂️ Methodology

### 1. Data Preprocessing & Cleaning
- Handled decimal separators and performed data type conversions
- Detected and treated outliers in physical variables (height and weight)
- Applied `StandardScaler` for feature normalization, ensuring proper convergence of the linear model

### 2. Exploratory Data Analysis (EDA)
- Used Boxplots and Violin Plots to visualize that **age** and **weight** are the most visually distinct risk factors between positive and negative groups
- Computed a correlation matrix to assess relationships between lifestyle habits (smoking, alcohol) and the target variable

### 3. Class Balancing (SMOTE)
- Applied **SMOTE** (Synthetic Minority Over-sampling Technique) to balance the training set to a 50/50 ratio
- Prevented the model from being biased toward the majority class

### 4. Model Training & Evaluation
- Algorithm: **Logistic Regression**
- Coefficient analysis revealed that **Age** and **Glucose level** were the strongest predictors for a positive diagnosis

---

## 📊 Results

| Metric | Value |
|---|---|
| Accuracy | 64% |
| AUC-ROC | 0.70 |
| Precision / Recall | Balanced — no significant overfitting |

> **Note:** The AUC-ROC of 0.70 represents a solid clinical baseline. Logistic Regression was chosen intentionally for its interpretability — understanding *why* a model makes a prediction is critical in healthcare contexts.

---

## 🛠️ Tech Stack

| Category | Tools |
|---|---|
| Language | Python |
| Data Manipulation | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn (Logistic Regression, StandardScaler) |
| Class Balancing | Imbalanced-learn (SMOTE) |
| Environment | Jupyter Notebook |

---

## ▶️ How to Run

```bash
# Clone the repository
git clone https://github.com/oporaxuao/cardiovascular-disease-logistic-regression.git
cd cardiovascular-disease-logistic-regression

# Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn jupyter

# Launch the notebook
jupyter notebook
```

---

## 👤 Author

**João Alfredo de Sousa Siqueira**
[![LinkedIn](https://img.shields.io/badge/LinkedIn-oporaxuao-blue)](https://linkedin.com/in/oporaxuao)
[![GitHub](https://img.shields.io/badge/GitHub-oporaxuao-black)](https://github.com/oporaxuao)
