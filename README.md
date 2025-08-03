# 💳 Loan Default Prediction

This project predicts whether a loan applicant will default using supervised machine learning techniques. The goal is to assist lenders in minimizing financial risk by accurately flagging high-risk borrowers.

---

## 🔍 Problem Statement

Predict whether a borrower will default (`1`) or not (`0`) based on financial, demographic, and behavioral features. In a lending scenario, **catching defaulters (high recall)** is far more important than simply maximizing accuracy.

---

## 🧠 Models Used

- **Logistic Regression** (Baseline, interpretable, threshold tuned)
- **Random Forest Classifier** (Ensemble benchmark)

Each model was evaluated using:
- Accuracy
- Precision
- Recall
- F1-Score

---

## 📊 Model Comparison

| Model                | Accuracy | Precision (Defaulters) | Recall (Defaulters) | F1-Score (Defaulters) |
|---------------------|----------|-------------------------|----------------------|------------------------|
| Logistic Regression | 76%      | 0.53                    | **0.72**             | **0.61**               |
| Random Forest        | **81%**  | **0.65**                | 0.49                 | 0.56                   |

> 🔎 **Conclusion:** Logistic Regression, despite slightly lower accuracy, had significantly **higher recall for defaulters**, which is more critical in credit risk management.

---

## 📈 Key Techniques

- **Threshold tuning** to improve recall without retraining
- **Classification report** & **confusion matrix** analysis
- **Precision-Recall trade-off** plotted and optimized
- **Random Forest** as a benchmark (sacrificed recall for higher precision)

---

## 🚀 How to Run

1. Open the notebook or script file
2. Ensure required libraries are installed (pandas, scikit-learn, etc.)
3. Run all cells or the script to train models and view evaluation results

---

## ✅ Future Improvements

- Try **XGBoost** or **LightGBM** for better non-linear performance
- Use **SMOTE** or **class_weight** tuning to handle class imbalance
- Deploy as a **Streamlit app** or **Flask API** for real-time prediction

---

## 🙋‍♂️ Author

Built by Pranav Dixit — part of a resume-linked ML projects portfolio.
