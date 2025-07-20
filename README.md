# 📊 Customer Churn Prediction – End-to-End ML Project

This project builds a complete Machine Learning pipeline to **predict customer churn** using real telecom data.

## 🔍 Objective

Predict whether a customer is likely to **leave the telecom service (churn)** based on their usage and profile.

---

## 📁 Dataset

**Source:** [Telco Customer Churn - Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)  
**Rows:** 7043 customers  
**Target Column:** `Churn` (Yes/No)

---

## 🧠 Model: XGBoost Classifier

- Tuned with `GridSearchCV`
- Evaluated with Accuracy, Confusion Matrix, and Classification Report
- Explained using **SHAP** and **LIME**

---

## ⚙️ Pipeline Steps

1. **Data Loading** using Pandas  
2. **Data Cleaning & Preprocessing**
   - Handled missing values
   - Encoded categorical variables
   - Converted `TotalCharges` to numeric
   - Target column: `Churn` → binary
3. **Train/Test Split**
4. **Model Training** with XGBoost + hyperparameter tuning
5. **Model Interpretation**
   - Global + Local explanations using **SHAP**
   - Individual prediction explained using **LIME**
6. **Saving Outputs**
   - Model saved as `.pkl`
   - Predictions saved as `.csv` and `.db`

---

## 📈 Results

- **Best Parameters:**  
  `n_estimators=50`, `learning_rate=0.1`, `max_depth=4`

- **Accuracy:** `79.3%`

- **Classification Report:**

| Class | Precision | Recall | F1-Score |
|-------|-----------|--------|----------|
| No Churn | 0.83 | 0.90 | 0.87 |
| Churn    | 0.65 | 0.49 | 0.56 |

---

## 📊 SHAP Interpretations

![SHAP Summary](images/shap_summary.png)  
*Explains which features most impacted predictions.*

---

## 📦 Files in Repo

| File                        | Description                         |
|----------------------------|-------------------------------------|
| `churn_model.pkl`          | Trained XGBoost model               |
| `churn_predictions.csv`    | Saved test predictions              |
| `churn_results.db`         | SQLite version of predictions       |
| `Telco-Customer-Churn.csv` | Raw dataset                         |
| `churn_notebook.ipynb`     | Full end-to-end ML notebook         |
| `README.md`                | This project overview               |

---

## ✅ Skills Demonstrated

- Data Cleaning & Preprocessing
- Feature Engineering
- XGBoost + Hyperparameter Tuning
- Model Interpretation (SHAP + LIME)
- SQLite Integration
- Git & GitHub project documentation

---

## 🚀 Author

**Sushma Sandanshiv**  
🔗 [LinkedIn](https://www.linkedin.com/in/sushma-sandanshiv-2740422b7/)  
💻 [GitHub](https://github.com/sushma-prog)

---

