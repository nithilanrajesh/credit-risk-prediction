# Credit Default Prediction – Interpretable Machine Learning (SHAP Project)

This project predicts **credit card default** using XGBoost and RandomForest models, followed by global and local interpretability using **SHAP (SHapley Additive exPlanations)**.

The project is structured according to explainable ML requirements for model transparency and fairness.

---

## 📂 Repository Structure

```
credit-default-shap-project/
│
├── project.ipynb
├── report.md
├── requirements.txt
├── default_credit.xls (or data file)
│
└── plots/
    ├── global_shap_summary.png
    ├── global_shap_bar.png
    ├── local_false_negative.png
    ├── local_false_positive.png
    └── local_borderline_correct.png
```

---

## 📊 Models Used
- **XGBoost Classifier**
- **RandomForest Classifier**

### Evaluation Metrics
- **AUC Score**
- **F1 Score**
- Confusion Matrix & Classification Report

---

## 🔍 Interpretability
This project uses **SHAP** for:

### ✔ Global Interpretability  
- Top 10 most important features  
- Summary plot  
- Feature importance bar plot  

### ✔ Local Interpretability  
- False Negative case  
- False Positive case  
- Borderline correct prediction  

---

## 🛠 How to Run the Project

### Option 1 — Google Colab (Recommended)
1. Upload the dataset and notebook  
2. Install packages using `requirements.txt`  
3. Run cells from top to bottom  

### Option 2 — Local Machine
```
pip install -r requirements.txt
jupyter notebook project.ipynb
```

---

## 🧠 Key Insights
- Payment history (PAY_0, PAY_2, PAY_3) and recent payment amounts (PAY_AMT6, PAY_AMT4) are leading predictors.
- SHAP reveals true feature influence more accurately than XGBoost built-in importance.
- Local explanations highlight model errors and risk patterns.

---

## 📞 Contact
If you have any questions about the project or execution, feel free to reach out.

---

