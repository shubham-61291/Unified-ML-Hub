# 🧠 Classification (Categorical Output) — All Models Overview

A unified collection of **supervised classification models** implemented by **Shubham Singh**, covering Binary, Multiclass, and Multilabel tasks.  
Each subfolder demonstrates end-to-end model pipelines — from data preprocessing and training to visualization and explainability.

---

## 🔗 Model Navigation
- [⚡ Gradient Boosting — XGBoost · LightGBM · CatBoost](#-gradient-boosting--xgboost--lightgbm--catboost-binary--multiclass-classification)
- [🤖 K-Nearest Neighbors (KNN)](#-k-nearest-neighbors-knn--binary-multiclass--multilabel-classification)
- [🧠 Neural Networks (Keras)](#-neural-networks-keras--binary-multiclass--multilabel-classification)
- [📊 Naïve Bayes (GaussianNB)](#-naïve-bayes-gaussiannb--binary-multiclass--multilabel-classification)
- [⚙️ Support Vector Machine (SVM)](#️-support-vector-machine-svm--binary-multiclass--multilabel-classification)
- [🌳 Decision Tree Classifier](#-decision-tree-classifier--binary-multiclass--multilabel)
- [⚖️ Logistic Regression](#️-logistic-regression--binary-multiclass--multilabel-classification)
- [🌲 Random Forest Classifier](#-random-forest-classifier--binary-multiclass--multilabel-classification)

---

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
![Confusion Matrix — XGBoost](./Gradient%20Boosting/confusion_matrix_xgboost.png)
![Confusion Matrix — LightGBM](./Gradient%20Boosting/confusion_matrix_GBM.png)
![Confusion Matrix — CatBoost](./Gradient%20Boosting/confusion_matrix_catboost.png)

### ROC & PR Curves
![ROC Curve — XGBoost](./Gradient%20Boosting/ROC_curve_xgboost.png)
![ROC Curve — LightGBM](./Gradient%20Boosting/ROC_PR_Curve_GBM.png)
![ROC Curve — CatBoost](./Gradient%20Boosting/ROC_PR_curve_catboost.png)

### Calibration Curves
![Calibration Curve — Binary](./Gradient%20Boosting/callibration_curve_GBM.png)

---

## 🌈 Multiclass Classification Results
![Confusion Matrix — Multiclass (CatBoost)](./Gradient%20Boosting/confusion_matrix_multiclass_catboost.png)
![ROC Curve — Multiclass (CatBoost)](./Gradient%20Boosting/ROC_curve_multiclass_catboost.png)
![PR Curve — Multiclass (CatBoost)](./Gradient%20Boosting/PR_curve_multiclass_catboost.png)

---

## 💡 Insights
- **XGBoost** performs best in recall and ROC-AUC.
- **LightGBM** provides faster convergence on GPU.
- **CatBoost** handles categorical features smoothly with strong calibration.

---

---

# 🤖 K-Nearest Neighbors (KNN) — Binary, Multiclass & Multilabel Classification

The **K-Nearest Neighbors (KNN)** algorithm is a non-parametric method used for classification and regression.  
This project demonstrates its application on **Binary**, **Multiclass**, and **Multilabel** datasets with full model evaluation and visualization.

---

## 🚀 Key Features
✅ Binary classification using **Breast Cancer Dataset**  
✅ Multiclass classification using **Iris Dataset**  
✅ Multilabel classification using **synthetic dataset**  
✅ Includes **ROC/PR curves**, **Calibration**, and **Confusion matrices**

---

## 📊 Binary Classification
![Confusion Matrix — Binary](./KNN/confusion_matrix_binary.png)
![ROC-PR Curve — Binary](./KNN/ROC_PR_Curve_binary.png)
![Threshold Tuning](./KNN/threshold_tuning_binary.png)
![Calibration Curve — Binary](./KNN/Calibration_curve_binary.png)

---

## 🌈 Multiclass Classification
![Confusion Matrix — Multiclass](./KNN/Confusion_matrix_multiclass.png)
![ROC Curve — Multiclass](./KNN/ROC_curve_multiclass.png)

---

## 🔢 Multilabel Classification
![Confusion Matrix — Multilabel Label 0](./KNN/confusion_matrix_label_0_multilabel.png)
![ROC Curve — Multilabel](./KNN/ROC_curve_multilabel.png)
![PR Curve — Multilabel](./KNN/PR_Curve_multilabel.png)

---

## 💡 Insights
- Interpretable model with no training phase.  
- **Binary:** High recall with threshold tuning.  
- **Multilabel:** Balanced precision-recall tradeoff.

---


---

# 🧠 Neural Networks (Keras) — Binary, Multiclass & Multilabel Classification

The **Neural Network (Keras)** model is a flexible deep-learning approach that learns nonlinear decision boundaries through layered representations.

---

## 🚀 Key Highlights
✅ TensorFlow 2.19 / Keras 2.19  
✅ Binary, Multiclass, Multilabel support  
✅ Visualizations: Learning Curves, Confusion Matrices, ROC & PR Curves  

---

## 📊 Binary Classification
![Learning Curve — Binary](./NN/learning_curve_binary.png)
![Confusion Matrix — Binary](./NN/confusion_matrix_binary.png)
![ROC-PR Curve — Binary](./NN/roc_pr_curve_binary.png)

---

## 🌈 Multiclass Classification
![Learning Curve — Multiclass](./NN/learning_curve_multiclass.png)
![Confusion Matrix — Multiclass](./NN/confusion_matrix_multiclass.png)
![ROC-PR Curve — Versicolor](./NN/roc_pr_curve_versicolor.png)

---

## 🔢 Multilabel Classification
![Learning Curve — Multilabel](./NN/learning_curve_multilabel.png)
![ROC-PR Curve — Label 0](./NN/roc_pr_curve_label0.png)
![ROC-PR Curve — Label 1](./NN/roc_pr_curve_label1.png)

---

## 💡 Insights
- **Binary:** AUC ≈ 0.99  
- **Multiclass:** Clear species separation  
- **Multilabel:** Balanced precision-recall with Hamming Loss ≈ 0.17  

---


---

# 📊 Naïve Bayes (GaussianNB) — Binary, Multiclass & Multilabel Classification

Implements **Naïve Bayes classifiers** for **Binary**, **Multiclass**, and **Multilabel** classification — complete with calibration, threshold tuning, and feature distribution visualization.

---

## 📊 Binary Classification
![Confusion Matrix — Binary](./Naïve%20Bayes/confusion_matrix_binary.png)
![ROC-PR Curve — Binary](./Naïve%20Bayes/roc_pr_curve_binary.png)
![Calibration Curve — Binary](./Naïve%20Bayes/calibration_curve_binary.png)

---

## 🌈 Multiclass Classification
![Confusion Matrix — Multiclass](./Naïve%20Bayes/confusion_matrix_multiclass.png)
![ROC Curve — Multiclass](./Naïve%20Bayes/roc_curve_multiclass.png)

---

## 🔢 Multilabel Classification
![Confusion Matrix — Label 0](./Naïve%20Bayes/confusion_matrix_label_0_multilabel.png)
![ROC Curve — Label 1](./Naïve%20Bayes/roc_curve_multilabel_label1.png)

---

## 💡 Insights
- **Binary:** GaussianNB aligns well with continuous distributions.  
- **Multiclass:** Probabilistic and interpretable.  
- **Multilabel:** Stable under label correlation.

---

---

# ⚙️ Support Vector Machine (SVM) — Binary, Multiclass & Multilabel Classification

Kernel-based classifier using **RBF** and **LinearSVC** variants.

---

## 📊 Binary Classification
![Confusion Matrix — Binary](./Support%20Vector%20Machines%20(SVM)/confusion_matrix_binary.png)
![ROC-PR Curve — Binary](./Support%20Vector%20Machines%20(SVM)/roc_pr_curve_binary.png)
![Calibration Curve — Binary](./Support%20Vector%20Machines%20(SVM)/calibration_curve_binary.png)

---

## 🌈 Multiclass Classification
![Confusion Matrix — Multiclass](./Support%20Vector%20Machines%20(SVM)/confusion_matrix_multiclass.png)
![ROC Curve — Multiclass](./Support%20Vector%20Machines%20(SVM)/roc_curve_multiclass.png)

---

## 🔢 Multilabel Classification
![Confusion Matrix — Label 0](./Support%20Vector%20Machines%20(SVM)/confusion_matrix_label0.png)
![ROC Curve — Label 2](./Support%20Vector%20Machines%20(SVM)/roc_curve_multilabel2.png)

---

## 💡 Insights
- Excellent **AUC ≈ 0.99** for binary case.  
- Clear class margins and separability in multiclass.

---


---

# 🌳 Decision Tree Classifier — Binary, Multiclass & Multilabel

Interpretable tree-based model covering all classification types.

---

## 📊 Binary Classification
![Confusion Matrix](./decission%20tree/confusionmatrix_binary.png)
![ROC-PR Curve](./decission%20tree/ROC_PRcurve_binary.png)
![Feature Importance](./decission%20tree/featureimportance_binary.png)

---

## 🌈 Multiclass Classification
![Confusion Matrix — Multiclass](./decission%20tree/confusionmatrix_multiclass.png)
![ROC Curve — Multiclass](./decission%20tree/roccurve_multiclass.png)
![Tree Visualization](./decission%20tree/decissiontree_multiclass.png)

---

## 🔢 Multilabel Classification
![Confusion Matrix Multilabel](./decission%20tree/confusionmatrix_multilabel.png)

---

## 💡 Insights
- Highly interpretable rules.  
- Great baseline model before ensembles.

---


---

# ⚖️ Logistic Regression — Binary, Multiclass & Multilabel Classification

Demonstrates **Logistic Regression** for all three classification settings.

---

## 📊 Binary Classification
![Confusion Matrix](./logistic%20regression/ConfusionMatrix.png)
![ROC Curve](./logistic%20regression/ROC_PRcurve.png)
![Threshold Tuning](./logistic%20regression/thresholdtuning.png)

---

## 🌈 Multiclass Classification
![Confusion Matrix — Multiclass](./logistic%20regression/confusion_matrixmulticlass.png)
![ROC Curve — Multiclass](./logistic%20regression/roc_curve_multiclass.png)

---

## 🔢 Multilabel Classification
![Confusion Matrix — Multilabel](./logistic%20regression/confusionmatrix_multilabel.png)

---

## 💡 Insights
- Excellent calibration and threshold tuning.  
- Robust generalization for all three classification types.

---


---

# 🌲 Random Forest Classifier — Binary, Multiclass & Multilabel Classification

Robust ensemble-based classifier improving over Decision Trees.

---

## 📊 Binary Classification
![Confusion Matrix — Binary](./random%20forest/confusion_matrix_binary.png)
![ROC-PR Curve — Binary](./random%20forest/roc_pr_curve_binary.png)
![Feature Importance](./random%20forest/feature_importance_binary.png)
![OOB Curve](./random%20forest/oob_score_vs_number_of_trees.png)

---

## 🌈 Multiclass Classification
![Confusion Matrix — Multiclass](./random%20forest/confusion_matrix_multiclass.png)
![ROC Curve — Multiclass](./random%20forest/roc_curves_multiclass.png)
![Feature Importance — Multiclass](./random%20forest/feature_importance_multiclass.png)

---

## 🔢 Multilabel Classification
![Confusion Matrix — Label 0](./random%20forest/confusion_matrix_multilabel_label0.png)
![Feature Importance — Multilabel](./random%20forest/feature_importance_multilabel.png)

---

## 💡 Insights
- AUC ≈ 0.99 for binary case.  
- Stable generalization across folds.  
- Consistent interpretability via permutation importance.

---

## 👨‍💻 Author
**Shubham Singh**

---

## 📜 License
MIT License
