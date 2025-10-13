# 🌲 Random Forest Classifier — Binary, Multiclass & Multilabel Classification

The **Random Forest** algorithm is a robust ensemble method that combines multiple decision trees to enhance accuracy, stability, and interpretability.  
This project demonstrates its implementation across **Binary**, **Multiclass**, and **Multilabel** problems, including detailed threshold optimization, feature importance, and calibration.

---

## 🚀 Key Highlights
✅ Applied Random Forest on three classification tasks (Binary, Multiclass, Multilabel)  
✅ Comprehensive evaluation: CV metrics, Confusion Matrices, ROC/PR Curves, Calibration Curves  
✅ **Threshold Tuning** with optimal thresholds table for Binary classification  
✅ **Feature Importance (MDI & Permutation)** with interpretive visualization  
✅ **OOB Curve** illustrating ensemble stability  

---

## 📊 Binary Classification — Breast Cancer Dataset

### Confusion Matrix  
![Confusion Matrix — Binary](confusion_matrix_binary.png)

### ROC & PR Curves  
![ROC-PR Curve — Binary](roc_pr_curve_binary.png)  
![ROC-PR Curve (Optima)](roc_pr_curve_binary_optima.png)

### Threshold Tuning  
![Threshold Tuning — Binary](threshold_tuning_binary.png)

### Calibration Curve  
![Calibration Curve — Binary](calibration_curve_binary.png)

### Feature Importance  
![Feature Importance — Binary](feature_importance_binary.png)

### Permutation Importance  
![Permutation Importance — Binary](permutation_importance_binary.png)

### OOB Curve  
![OOB Score vs Number of Trees](oob_score_vs_number_of_trees.png)

---

## 🌈 Multiclass Classification — Iris Dataset

### Confusion Matrix  
![Confusion Matrix — Multiclass](confusion_matrix_multiclass.png)

### ROC & PR Curves  
![ROC Curves — Multiclass](roc_curves_multiclass.png)  
![PR Curves — Multiclass](pr_curve_multiclass.png)

### Feature Importance  
![Feature Importance — Multiclass](feature_importance_multiclass.png)

### Permutation Importance  
![Permutation Importance — Multiclass](permutation_importance_multiclass.png)

---

## 🔢 Multilabel Classification — Synthetic Dataset

### Confusion Matrix (Label 0)  
![Confusion Matrix — Label 0 Multilabel](confusion_matrix_multilabel_label0.png)

### Feature Importance  
![Feature Importance — Multilabel](feature_importance_multilabel.png)

---

## 🧮 Model Performance Summary

| Task | Dataset | Accuracy | F1 | AUC | Hamming | Jaccard |
|------|----------|-----------|----|------|----------|----------|
| Binary | Breast Cancer | 0.95 | 0.96 | 0.99 | — | — |
| Multiclass | Iris | 0.91 | 0.91 | — | — | — |
| Multilabel | Synthetic | — | 0.66 | — | 0.19 | 0.50 |

---

## 🔬 Insights
- **Binary:** Strong generalization with AUC ≈ 0.99 and stable OOB score (0.967).  
- **Multiclass:** Excellent separation across Iris classes with consistent F1 scores.  
- **Multilabel:** Demonstrates balanced precision-recall with moderate label overlap.  
- **Feature Importance:** Identifies key features via both MDI and permutation metrics.  

---

## 🔮 Future Enhancements
- Integrate **GridSearchCV** or **Optuna** for hyperparameter tuning  
- Add **SHAP** interpretability plots  
- Extend to **Regression** and **Imbalanced Classification** scenarios  

---

## 👨‍💻 Author
**Shubham Singh**

---

## 📜 License
MIT License
