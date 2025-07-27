# CodeAlpha_CreditScoringModel
## 🧠 Project Title: Credit Scoring Model
This project is part of the **CodeAlpha Machine Learning Internship**. The goal is to build a **Credit Scoring Model** that predicts whether a transaction (or user) is creditworthy using financial data.
## 📦 Dataset
We used the [Kaggle Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud), which contains anonymized financial transactions.
 **Rows**: 284,807 transactions
- **Features**: 30 (V1–V28 from PCA, Time, Amount)
- **Target**: `Class` (0 = Non-Fraud / Creditworthy, 1 = Fraud / Not Creditworthy)

## ⚙️ Technologies Used

- Python 3
- Pandas, NumPy
- Scikit-learn
- Imbalanced-learn (SMOTE)
- Matplotlib, Seaborn
## 🧹 Preprocessing Steps

- Removed class imbalance using **SMOTE**
- Scaled `Time` and `Amount` using `StandardScaler`
- Split data into training and testing sets
- Handled class imbalance with stratified sampling
## 🤖 Models Used

| Model               | Evaluation Metric |
|--------------------|--------------------|
| Logistic Regression | Accuracy, F1-Score |
| Decision Tree       | Accuracy, F1-Score |
| ✅ Random Forest (Best) | F1-Score, ROC-AUC |

---

## 🔍 Evaluation Metrics

- **Precision**
- **Recall**
- **F1-Score**
- **ROC-AUC Score**

```python
Classification Report:
Precision, Recall, F1-Score for both classes

ROC-AUC Score: > 0.98 ✅
