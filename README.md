# 📈 Credit Risk Classification Report – Custom Version

## 🧠 Overview

The goal of this analysis is to evaluate the performance of a **Logistic Regression** model in predicting the likelihood of loan default using a dataset from a peer-to-peer lending platform. This helps financial analysts assess borrower creditworthiness and reduce risk.

---

## 🔍 Dataset Overview

- **Features used:**  
  - loan_size  
  - interest_rate  
  - borrower_income  
  - debt_to_income  
  - number_of_open_accounts  
  - derogatory_marks  
  - total_debt  

- **Target Variable:**  
  - `loan_status` (0 = healthy loan, 1 = high-risk loan)

---

## 📊 Results

- **Accuracy Score:** 0.99
- **Precision:**
  - Class 0 (Healthy Loan): 1.00  
  - Class 1 (High Risk): 0.85
- **Recall:**
  - Class 0: 0.99  
  - Class 1: 0.91

These metrics were obtained from evaluating the logistic regression model on test data after splitting the dataset.

---

## 🧪 Model Summary

The logistic regression classifier achieved strong results, especially in predicting healthy loans (Class 0) with nearly perfect precision and recall.

For high-risk loans (Class 1), the precision and recall are solid, though not perfect. This suggests some false positives, meaning the model might occasionally label a safe loan as risky. However, the high recall (0.91) shows that it identifies most risky loans correctly.

---

## ✅ Recommendation

The model performs reliably on this dataset. It is suitable as a first-pass tool to flag high-risk loans for further manual review. For production deployment, additional model validation on newer or more diverse data is recommended.

---

## 💡 Future Improvements

- Apply resampling techniques (e.g., SMOTE) to address class imbalance
- Try alternate models (e.g., Random Forest, XGBoost) for comparison
- Perform feature engineering and correlation analysis
