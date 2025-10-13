# 🤖 K-Nearest Neighbors (KNN) — Binary, Multiclass & Multilabel Classification

The **K-Nearest Neighbors (KNN)** algorithm is a non-parametric method used for classification and regression.  
This project demonstrates its application on **Binary**, **Multiclass**, and **Multilabel** datasets with full model evaluation and visualization.

---

## 🚀 Key Features
✅ Binary classification using the **Breast Cancer Dataset**  
✅ Multiclass classification using the **Iris Dataset**  
✅ Multilabel classification using a **synthetic dataset**  
✅ Includes **ROC/PR curves**, **Calibration curves**, **Threshold tuning**, and **Confusion matrices**  
✅ Visual performance analysis through **k-vs-error** and **subset accuracy** plots  

---

## 📊 Binary Classification (Breast Cancer Dataset)

### Confusion Matrix  
![Confusion Matrix — Binary](confusion_matrix_binary.png)

### ROC & PR Curves  
![ROC-PR Curve — Binary](ROC_PR_Curve_binary.png)  
![Optimized ROC-PR Curve](ROC_PR_optima.png)

### Threshold Tuning  
![Threshold Tuning — Binary](threshold_tuning_binary.png)

### Calibration Curve  
![Calibration Curve — Binary](Calibration_curve_binary.png)

### k-vs-Error Curve  
![k vs Error — Binary](Kvserror_binary.png)

---

## 🌈 Multiclass Classification (Iris Dataset)

### Confusion Matrix  
![Confusion Matrix — Multiclass](Confusion_matrix_multiclass.png)

### ROC & PR Curves  
![ROC Curve — Multiclass](ROC_curve_multiclass.png)  
![PR Curve — Multiclass](PR_curve_multiclass.png)

### Calibration Curve  
![Calibration Curve — Multiclass](calibration_curve_multiclass.png)

---

## 🔢 Multilabel Classification (Synthetic Dataset)

### Confusion Matrix (Label 0)  
![Confusion Matrix — Multilabel Label 0](confusion_matrix_label_0_multilabel.png)

### ROC Curves  
![ROC Curve — Multilabel](ROC_curve_multilabel.png)  
![ROC Curve — Multilabel Label 2](ROC_curve_multilabel_abel_2.png)  
![ROC Curve — Multilabel Fork9](ROC_curve_multilabel_fork9.png)

### PR Curves  
![PR Curve — Multilabel](PR_Curve_multilabel.png)  
![PR Curve — Multilabel Label 2](PR_curve_multilabel_label_2.png)

### Subset Accuracy  
![Subset Accuracy — Multilabel](KvsSubset_accuracy_multilabel.png)

---

## 💡 Insights
- **KNN** provides interpretable decision boundaries without explicit training.  
- **Binary**: High recall with optimized thresholds.  
- **Multiclass**: Excellent separation among classes.  
- **Multilabel**: Balanced precision and recall across correlated outputs.  

---

## 🔮 Future Enhancements
- Add **distance weighting** (uniform vs distance) analysis  
- Compare **KNN vs SVM** for similar datasets  
- Extend to **regression tasks**  
- Implement **KD-Tree / Ball-Tree acceleration** for scalability  

---

## 👨‍💻 Author
**Shubham Singh**

---

## 📜 License
MIT License
