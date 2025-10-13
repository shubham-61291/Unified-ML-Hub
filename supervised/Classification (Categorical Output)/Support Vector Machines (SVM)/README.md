# ⚙️ Support Vector Machine (SVM) — Binary, Multiclass & Multilabel Classification

The **Support Vector Machine (SVM)** algorithm is a powerful kernel-based method that finds the optimal separating hyperplane between classes.  
This project demonstrates the application of **SVM (RBF kernel)** and **LinearSVC** across **Binary**, **Multiclass**, and **Multilabel** classification tasks, showcasing model tuning, evaluation, and visualization.

---

## 🚀 Key Highlights
✅ Implemented with both **RBF** and **LinearSVC** variants  
✅ Applied on Binary, Multiclass, and Multilabel datasets  
✅ Includes **5-fold Cross-Validation**, **ROC/PR Curves**, and **Calibration** plots  
✅ **Threshold Tuning** with optimal thresholds (F1-max, J-max, Cost-min)  
✅ Detailed **Confusion Matrices** and **Per-Class Calibration Curves**

---

## 📊 Binary Classification — Breast Cancer Dataset

### Confusion Matrix  
![Confusion Matrix — Binary](confusion_matrix_binary.png)

### ROC & PR Curves  
![ROC-PR Curve — Binary](roc_pr_curve_binary.png)  
![ROC-PR Curve — Optima](roc_pr_curve_binary_optima.png)

### Threshold Tuning  
![Threshold Tuning — Binary](threshold_tuning_binary.png)

### Calibration Curve  
![Calibration Curve — Binary](calibration_curve_binary.png)

---

## 🌈 Multiclass Classification — Iris Dataset

### Confusion Matrix  
![Confusion Matrix — Multiclass](confusion_matrix_multiclass.png)

### ROC & PR Curves  
![ROC Curve — Multiclass](roc_curve_multiclass.png)  
![PR Curve — Multiclass](pr_curve_multiclass.png)

### Calibration Curves (Per Class)  
![Calibration Curves — Setosa, Versicolor, Virginica](calibration_sentosa_versicolor_virginica.png)

---

## 🔢 Multilabel Classification — Synthetic Dataset

### Confusion Matrix (Label 0)  
![Confusion Matrix — Label 0](confusion_matrix_label0.png)

### ROC Curves (per label)  
![ROC Curve — Label 0](roc_curve_multilabel0.png)  
![ROC Curve — Label 1](roc_curve_multilabel1.png)  
![ROC Curve — Label 2](roc_curve_multilabel2.png)

### PR Curves (per label)  
![PR Curve — Label 0](pr_curve_multilabel0.png)  
![PR Curve — Label 1](pr_curve_multilabel1.png)  
![PR Curve — Label 2](pr_curve_multilabel2.png)

---

## 🧮 Model Performance Summary

| Task | Dataset | Accuracy | F1 | AUC | Hamming | Jaccard |
|------|----------|-----------|----|------|----------|----------|
| Binary | Breast Cancer | 0.98 | 0.98 | 0.99 | — | — |
| Multiclass | Iris | 0.93 | 0.93 | — | — | — |
| Multilabel | Synthetic | — | 0.69 | — | 0.186 | 0.528 |

---

## 🔬 Insights
- **Binary (RBF SVM):** Achieved 98% accuracy and AUC ≈ 0.99 with excellent calibration.  
- **Multiclass:** High precision across species with clear OvR separation.  
- **Multilabel:** Balanced F1 across labels, effective under moderate correlation.  
- **Threshold Optimization:** Cost-based tuning reduces false negatives under asymmetric penalties.

---

## 🔮 Future Enhancements
- Integrate **Polynomial** and **Sigmoid kernels** for comparison  
- Use **GridSearchCV / Optuna** for hyperparameter tuning  
- Incorporate **SHAP** and **LIME** explainability visualizations  

---

## 👨‍💻 Author
**Shubham Singh**

---

## 📜 License
MIT License
