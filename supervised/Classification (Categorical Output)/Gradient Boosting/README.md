# ⚡ Gradient Boosting: XGBoost · LightGBM · CatBoost

A comprehensive notebook showcasing **Gradient Boosting** for  
1️⃣ Binary Classification (Breast Cancer),  
2️⃣ Multiclass Classification (Iris), and  
3️⃣ Multilabel Classification (Synthetic dataset).

Includes all essential components — **CV metrics**, **threshold tuning**, **ROC/PR curves**, **calibration**, **permutation & SHAP explainability**, and **early stopping**.

---

## 🚀 Key Highlights

| Type | Models | Special Features |
|:-----|:--------|:----------------|
| Binary | XGBoost · LightGBM · CatBoost | Threshold tuning (F1-max / J-max / Cost-min), ROC/PR annotation, Calibration, SHAP |
| Multiclass | XGBoost · LightGBM · CatBoost | One-vs-Rest ROC/PR curves, per-class calibration, permutation importances |
| Multilabel | OvR(XGBoost/LightGBM/CatBoost) | Jaccard & Hamming metrics, per-label ROC/PR curves, mean feature importance |

---

## 📊 Binary Classification (Breast Cancer)

### 🔹 Mean 5-Fold CV Metrics (XGBoost)
| Metric | Mean ± SD |
|:--------|:-----------|
| Accuracy | 0.963 ± 0.010 |
| Precision | 0.968 ± 0.022 |
| Recall | 0.975 ± 0.022 |
| F1 | 0.971 ± 0.008 |
| ROC-AUC | 0.994 ± 0.005 |
| Log Loss | −0.098 ± 0.031 |

### 🔹 Optimal Thresholds (XGBoost)
| Criterion | Threshold | Precision | Recall | F1 | Youden-J | Cost |
|:-----------|:-----------:|:-----------:|:------:|:------:|:-----------:|:------:|
| F1-max | 0.395 | 0.955 | 1.000 | 0.977 | 0.922 | 5 |
| J-max | 0.533 | 0.964 | 0.991 | 0.977 | 0.928 | 14 |
| Cost-min | 0.395 | 0.955 | 1.000 | 0.977 | 0.922 | 5 |

---

## 📈 Binary Evaluation Visuals

- Confusion Matrix  
  ![Confusion Matrix](Confusionmatrixbinary.png)

- ROC/PR Curves  
  ![ROC-PR Curve](ROC_PRcurveXGboost_binary.png)  
  ![ROC/PR Optima](ROC_PRcurve_optima.png)

- Threshold Tuning  
  ![Threshold Tuning](threshold_binary.png)

- Calibration Curve  
  ![Calibration Curve](calibrationcurve_binary.png)

- Top Feature Importances  
  ![Top Feature Importance](topfeatureimp_binary.png)

- Permutation Importance  
  ![Permutation Importance](permutationimp_binary.png)

- SHAP Summary  
  ![SHAP Summary](SHAP_binary.png)

---

## 🌈 Multiclass (Iris)

### 🔹 Mean 5-Fold CV Metrics (LightGBM)
| Metric | Mean ± SD |
|:--------|:-----------|
| Accuracy | 0.953 ± 0.034 |
| F1 Macro | 0.953 ± 0.034 |
| F1 Micro | 0.953 ± 0.034 |
| Log Loss | −1.682 ± 1.225 |

- Multiclass ROC/PR Curves (OvR)  
  ![ROC Multiclass](ROC_PRcurve_optima.png)

- Feature Importance  
  ![Top Feature Importance](topfeatureimp_binary.png)

---

## 🔮 Multilabel (Synthetic Dataset, OvR)

| Metric | Value |
|:-------|:------:|
| Subset Accuracy | 0.18 |
| Hamming Loss | 0.280 |
| Jaccard (Micro) | 0.413 |

📊 Per-Label ROC/PR Curves and averaged feature importances highlight label-wise predictive patterns.

---

## 💡 Insights
- **XGBoost** achieves highest recall and calibration consistency.  
- **LightGBM** offers faster convergence and better cross-entropy.  
- **CatBoost** handles categorical and class imbalance elegantly.  
- **SHAP & Permutation plots** confirm feature robustness across variants.

---

## 🧠 Architecture Diagram
