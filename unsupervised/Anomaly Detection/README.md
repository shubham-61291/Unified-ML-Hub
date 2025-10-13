# 🧠 Anomaly Detection — Isolation Forest, One-Class SVM, Autoencoder & Statistical Baselines

This project demonstrates **unsupervised anomaly detection** using classical and neural approaches on synthetic data with injected outliers.  
It includes complete visual analysis — ROC, PR, Threshold Tuning, and Comparative Evaluation.

---

## 🚀 Key Highlights
✅ Implements five anomaly-detection techniques:
- **Isolation Forest**
- **One-Class SVM (RBF)**
- **Autoencoder (Neural Reconstruction Error)**
- **Z-Score Baseline**
- **Mahalanobis Distance**

✅ Synthetic dataset generation with injected anomalies  
✅ Unified evaluation framework for AUC-ROC, AUC-PR, and F1  
✅ Comprehensive visualization of model thresholds and distributions  
✅ PCA-based 2D visualization for Autoencoder and Isolation Forest  
✅ Comparative summary by AUC and F1

---

## ⚙️ Models & Results Overview

| Model | AUC-ROC | AUC-PR | F1 | Notes |
|--------|----------|--------|----|--------|
| Mahalanobis Distance | **0.9503** | **0.9056** | **0.9048** | Most stable with low variance |
| Autoencoder Reconstruction Error | 0.9234 | 0.7728 | 0.7381 | Learns deep nonlinear structure |
| One-Class SVM | 0.8991 | 0.7696 | 0.7381 | Kernel-based decision boundary |
| Isolation Forest | 0.8629 | 0.7324 | 0.7143 | Fast, tree-based ensemble |
| Z-Score Baseline | 0.8593 | 0.7254 | 0.7143 | Simple statistical cutoff |

---

## 🌲 Isolation Forest

### ROC Curve  
![ROC Curve — Isolation Forest](roc_curve_isolation_forest.png)

### Precision-Recall Curve  
![PR Curve — Isolation Forest](precission_recall_curve_isolation_forest.png)

### Threshold Optimization  
![Threshold Optimization — Isolation Forest](isolated_forest_threshold_optimization.png)

### Score Distribution  
![Score Distribution — Isolation Forest](isolation_forest_score_distribution.png)

---

## ⚙️ One-Class SVM

### ROC Curve  
![ROC Curve — One Class SVM](roc_curve_one_class_svm.png)

### Precision-Recall Curve  
![PR Curve — One Class SVM](precision_recall_curve_one_class_svm.png)

### Score Distribution  
![Score Distribution — One Class SVM](one_class_svm_score_distribution.png)

---

## 🧩 Autoencoder (Neural Network)

### Training Loss  
![Autoencoder Training Loss](autoencoder_training_loss.png)

### ROC Curve  
![ROC Curve — Autoencoder](roc_curve_autoencoder_reconstruction_error.png)

### Precision-Recall Curve  
![PR Curve — Autoencoder](precision_recall_curve_autoencoder_reconstruction_error.png)

### Threshold Optimization  
![Threshold Optimization — Autoencoder](autoencoder_threshold_optimization.png)

### Score Distribution  
![Score Distribution — Autoencoder](autoencoder_reconstruction_error_score_distribution.png)

---

## 📊 Statistical Baselines

### Z-Score Baseline  
![Z-Score ROC](roc_curve_z_score_baseline.png)  
![Z-Score PR](precision_recall_curve_z_score_baseline.png)  
![Z-Score Distribution](z_score_baseline_score_distribution.png)

### Mahalanobis Distance  
![Mahalanobis ROC](roc_curve_mahalanobis_distance.png)  
![Mahalanobis PR](precision_recall_curve_mahalanobis_distance.png)  
![Mahalanobis Distribution](mahalanobis_distance_score_distribution.png)

---

## 📈 Comparative Evaluation

### AUC-ROC Comparison  
![Model Comparison by AUC-ROC](model_comparison_by_auc_roc.png)

### F1 Comparison  
![Model Comparison by F1](model_comparison_by_f1.png)

---

## 🧮 Key Insights

- **Mahalanobis Distance** achieved the highest overall performance (AUC ≈ 0.95, F1 ≈ 0.90).  
- **Autoencoder** captured nonlinear patterns well, competitive with SVM.  
- **Z-Score** remains a strong baseline for high-dimensional data.  
- Ensemble and neural methods outperform classical baselines when data contain complex dependencies.  

---

## 🔮 Future Enhancements
- Integrate **Variational Autoencoder (VAE)** and **Deep SVDD** for richer representation learning  
- Use **t-SNE or UMAP** for high-dimensional projection  
- Add **real-world datasets** like KDD99 or NAB for evaluation  

---

## 👨‍💻 Author
**Shubham Singh**

---

## 📜 License
MIT License
