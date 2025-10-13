# ⚡ Gradient Boosting — XGBoost · LightGBM · CatBoost

This project demonstrates **GPU-accelerated Gradient Boosting** for  
1️⃣ Binary Classification (Breast Cancer)  
2️⃣ Multiclass Classification (Iris)  
3️⃣ Multilabel Classification (Synthetic dataset)

The notebook benchmarks **XGBoost**, **LightGBM**, and **CatBoost** across all three tasks, covering metrics, threshold tuning, calibration, feature importance, and SHAP explainability.

---

## 🚀 Key Features
- 5-Fold Cross-Validation (Accuracy, Precision, Recall, F1, ROC-AUC)
- GPU acceleration for all models (`tree_method="gpu_hist"`, `device="gpu"`)
- **Threshold tuning** (F1-max, Youden’s J, Cost-min)
- **Calibration curves**, **ROC/PR curves**, **Permutation importance**
- **SHAP summaries** for explainability
- Binary, multiclass, and multilabel benchmarks with comparative results

---

## 📊 Binary Classification (Breast Cancer)

| Model | Accuracy | Precision | Recall | F1 | ROC AUC |
|:------|:---------:|:----------:|:------:|:------:|
| **XGBoost** | 0.970 ± 0.012 | 0.973 ± 0.023 | 0.980 ± 0.011 | 0.976 ± 0.009 | 0.994 ± 0.005 |
| **LightGBM** | 0.968 ± 0.020 | 0.965 ± 0.027 | 0.986 ± 0.015 | 0.975 ± 0.016 | 0.992 ± 0.007 |
| **CatBoost** | 0.965 ± 0.019 | 0.962 ± 0.027 | 0.983 ± 0.011 | 0.972 ± 0.015 | 0.995 ± 0.004 |

✅ **Optimal Thresholds (XGBoost):**
- F1-max → 0.395  
- J-max → 0.533  
- Cost-min → 0.395  

---

### Binary Visuals
![Confusion Matrix](Confusionmatrixbinary.png)
![ROC/PR Curves](ROC_PRcurveXGboost_binary.png)
![ROC/PR Optima](ROC_PRcurve_optima.png)
![Threshold Tuning](threshold_binary.png)
![Calibration Curve](calibrationcurve_binary.png)
![Feature Importance](topfeatureimp_binary.png)
![Permutation Importance](permutationimp_binary.png)
![SHAP Summary](SHAP_binary.png)

---

## 🌈 Multiclass Classification (Iris)

| Model | Accuracy | F1 Macro |
|:------|:---------:|:--------:|
| **XGBoost** | 0.940 ± 0.033 | 0.939 ± 0.034 |
| **LightGBM** | 0.953 ± 0.034 | 0.953 ± 0.035 |
| **CatBoost** | 0.960 ± 0.025 | 0.960 ± 0.025 |

![Confusion Matrix (Multiclass)](confusionmatrix_multiclass.png)
![ROC Curves (OvR)](roccurve_multiclass.png)
![PR Curves (OvR)](prcurve_multiclass.png)

---

## 🧩 Multilabel Classification (Synthetic)

| Model | Subset Accuracy | Hamming Loss | Jaccard (Micro) |
|:------|:----------------:|:-------------:|:----------------:|
| **XGBoost** | 0.421 | 0.181 | 0.546 |
| **LightGBM** | 0.405 | 0.184 | 0.539 |
| **CatBoost** | 0.422 | 0.179 | 0.540 |

![Confusion Matrix (Multilabel)](confusionmatrix_multilabel.png)
![Feature Importance (Multilabel)](featureimportance_multilabel.png)

---

## 💡 Insights
- **XGBoost** yields the best calibration and recall stability.  
- **LightGBM** converges faster with efficient GPU usage.  
- **CatBoost** excels in handling categorical and imbalanced data.  
- SHAP confirms consistent feature importance across models (e.g., mean radius, worst area).

---

## 🔮 Future Enhancements
- Add **ensemble stacking** across GBMs.  
- Integrate **Optuna/Bayesian tuning** for hyperparameter optimization.  
- Extend SHAP interpretation to **multilabel outputs**.  

---

## 👨‍💻 Author
**Shubham Singh**

---

## 📜 License
MIT License
