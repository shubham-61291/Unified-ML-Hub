# 🧠 Naïve Bayes (GaussianNB) — Binary, Multiclass & Multilabel Classification

This project implements **Naïve Bayes classifiers** (GaussianNB) for three tasks — **Binary**, **Multiclass**, and **Multilabel** classification — demonstrating their behavior with detailed evaluation metrics, calibration, and visualization.

---

## 🚀 Key Highlights
✅ GaussianNB applied across Binary, Multiclass, and Multilabel datasets  
✅ Includes Cross-Validation (5-fold), ROC/PR Curves with annotated thresholds  
✅ Calibration curves for model reliability assessment  
✅ Feature distribution plots to validate Gaussian assumptions  
✅ Optimal Threshold Table and Cost Function visualization (Binary)  

---

## 📊 Binary Classification — Breast Cancer Dataset

### Confusion Matrix
![Confusion Matrix — Binary](confusion_matrix_binary.png)

### ROC & PR Curves
![ROC-PR Curve — Binary](roc_pr_curve_binary.png)
![Initial ROC-PR Curve — Binary](roc_pr_curve_binary_initial.png)

### Threshold Tuning
![Threshold Tuning — Binary](threshold_tuning_binary.png)

### Calibration Curve
![Calibration Curve — Binary](calibration_curve_binary.png)

### Feature Distributions
![Feature Distribution — Mean Area (Binary)](featuredist_meanarea_binary.png)
![Feature Distribution — Mean Perimeter](feature_dist_mean_perimeter.png)
![Feature Distribution — Mean Radius](feature_dist_mean_radius.png)

---

## 🌈 Multiclass Classification — Iris Dataset

### Confusion Matrix
![Confusion Matrix — Multiclass](confusion_matrix_multiclass.png)

### ROC & PR Curves
![ROC Curve — Multiclass](roc_curve_multiclass.png)
![PR Curve — Multiclass](pr_curve_multiclass.png)

### Calibration Curves
![Calibration Curve (Setosa vs Versicolor vs Virginica)](calibration_setosa_ver_vir.png)

### Feature Distributions
![Feature Distribution — Sepal Length](feature_dist_sepal_len.png)
![Feature Distribution — Petal Length](feature_dist_petal_len.png)

---

## 🔢 Multilabel Classification — Synthetic Dataset

### Confusion Matrix (Label 0)
![Confusion Matrix — Label 0 Multilabel](confusion_matrix_label_0_multilabel.png)

### ROC Curves (per label)
![ROC Curve — Multilabel Label 0](roc_curve_multilabel_label0.png)
![ROC Curve — Multilabel Label 1](roc_curve_multilabel_label1.png)
![ROC Curve — Multilabel Label 2](roc_curve_multilabel_label2.png)

### PR Curves (per label)
![PR Curve — Multilabel Label 0](pr_curve_multilabel_label0.png)
![PR Curve — Multilabel Label 1](pr_curve_multilabel_label1.png)
![PR Curve — Multilabel Label 2](pr_curve_multilabel_label2.png)

---

## 🧮 Model Performance Summary

| Task | Dataset | Accuracy | F1 | AUC | Hamming | Jaccard |
|------|----------|-----------|----|------|----------|----------|
| Binary | Breast Cancer | 0.95 | 0.96 | 0.989 | — | — |
| Multiclass | Iris | 0.91 | 0.91 | — | — | — |
| Multilabel | Synthetic | — | 0.68 | — | 0.201 | 0.520 |

---

## 🔬 Insights
- **Binary:** Excellent separability and calibration; GaussianNB aligns with breast cancer feature distribution.  
- **Multiclass:** Clear probabilistic decision boundaries for each Iris species.  
- **Multilabel:** Maintains balanced precision-recall tradeoff across multiple correlated labels.  

---

## 🔮 Future Enhancements
- Implement **BernoulliNB** and **MultinomialNB** variants for discrete data  
- Extend to **text classification** with TF-IDF features  
- Add **Bayesian hyperparameter tuning** for prior adjustment  

---

## 👨‍💻 Author
**Shubham Singh**

---

## 📜 License
MIT License
