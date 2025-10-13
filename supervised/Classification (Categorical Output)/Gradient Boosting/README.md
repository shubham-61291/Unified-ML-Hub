# ⚡ Gradient Boosting — XGBoost · LightGBM · CatBoost (Binary & Multiclass Classification)

This project showcases **Gradient Boosted Models (GBMs)** — including **XGBoost**, **LightGBM**, and **CatBoost** — for both **binary** and **multiclass** classification problems.

It includes complete evaluation pipelines: cross-validation, ROC/PR curves, confusion matrices, calibration, and interpretability using **SHAP** and **Permutation Importance**.

---

## 🚀 Key Highlights
- Implemented and compared **XGBoost**, **LightGBM**, and **CatBoost**
- Covers both **Binary** and **Multiclass** classification tasks
- 5-Fold CV with metrics: Accuracy, Precision, Recall, F1, ROC-AUC
- **Threshold tuning** and **probability calibration**
- **Feature importance** & **SHAP explainability**
- GPU acceleration enabled (`tree_method='gpu_hist'`, `device='gpu'`)

---

## 📊 Binary Classification Results

### Confusion Matrices
![Confusion Matrix — XGBoost](confusion_matrix_xgboost.png)
![Confusion Matrix — LightGBM](confusion_matrix_GBM.png)
![Confusion Matrix — CatBoost](confusion_matrix_catboost.png)
![Confusion Matrix — Binary](confusion_matrix_binary.png)

---

### ROC & PR Curves
![ROC Curve — XGBoost](ROC_curve_xgboost.png)
![ROC Curve — LightGBM](ROC_PR_Curve_GBM.png)
![ROC Curve — CatBoost](ROC_PR_curve_catboost.png)
![ROC Curve — Binary](ROC_PR_curve_binary.png)

![PR Curve — XGBoost](PR_curve_xgboost.png)
![PR Curve — Multiclass](PR_curvr_multiclass.png)
![PR Curve — CatBoost](PR_curve_multiclass_catboost.png)

---

### Calibration Curves
![Calibration Curve — Binary](calibration_curve_binary.png)
![Calibration Curve — CatBoost](calibration_curve_catboost.png)
![Calibration Curve — LightGBM](callibration_curve_GBM.png)

---

## 🌈 Multiclass Classification Results

### Confusion Matrices
![Confusion Matrix — Multiclass (XGBoost)](confusion_matrix_xgboost.png)
![Confusion Matrix — Multiclass (CatBoost)](confusion_matrix_multiclass_catboost.png)
![Confusion Matrix — Multiclass (General)](confusion_matrix_multiclass.png)

---

### ROC & PR Curves (Multiclass)
![ROC Curve — Multiclass (XGBoost)](ROC_curve_xgboost.png)
![ROC Curve — Multiclass (CatBoost)](roc_curve_multiclass_catboost.png)
![PR Curve — Multiclass (CatBoost)](PR_curve_multiclass_catboost.png)

---

## 💡 Insights
- **XGBoost** performs best in recall and ROC-AUC.
- **LightGBM** provides faster convergence on GPU.
- **CatBoost** handles categorical features smoothly with strong calibration.
- Model performance remains consistent across folds.

---

## 🧩 Future Enhancements
- Add **Optuna tuning** for automated hyperparameter search  
- Integrate **SHAP interaction values** for feature synergy analysis  
- Add **ensemble stacking** combining XGBoost + CatBoost  

---

## ⚙️ Dependencies
Refer to `requirements.txt` for all dependencies.

---

## 👨‍💻 Author
**Shubham Singh**

---

## 📜 License
MIT License

