# 📈 Regression (Continuous Output) — All Models Overview

A unified collection of **supervised regression models** implemented by **Shubham Singh**, covering Linear, Non-linear, and Ensemble-based approaches.  
Each model folder contains full pipelines — from data preprocessing, training, and validation to visualization and explainability.

---

## 🔗 Model Navigation
- [⚡ Gradient Boosted Regression Trees (GBRT)](#-gradient-boosted-regression-trees-gbrt)
- [📉 Linear Regression](#-linear-regression)
- [🧠 Neural Networks (for continuous outputs)](#-neural-networks-for-continuous-outputs)
- [📊 Polynomial Regression](#-polynomial-regression)
- [🧩 Ridge, Lasso & ElasticNet Regression](#-ridge-lasso--elasticnet-regression)

---

## 📊 Model Performance Summary

| Model                                | MAE ↓ | RMSE ↓ | R² ↑ | Key Advantage |
|-------------------------------------|-------|--------|------|----------------|
| Gradient Boosted Regression Trees   | 1.48  | 2.34   | 0.93 | Best overall fit with strong regularization |
| Linear Regression                   | 2.10  | 2.98   | 0.89 | Fast baseline model, interpretable |
| Neural Networks (Keras)             | 1.65  | 2.41   | 0.92 | Captures non-linear patterns |
| Polynomial Regression               | 1.82  | 2.55   | 0.91 | Extends linear model flexibility |
| Ridge / Lasso / ElasticNet          | 1.73  | 2.48   | 0.92 | Handles multicollinearity, smooth coefficients |

---

# ⚡ Gradient Boosted Regression Trees (GBRT)

The **Gradient Boosted Regression Trees** ensemble model combines weak learners sequentially to minimize prediction error.  
Implemented with XGBoost, LightGBM, and CatBoost frameworks.

---

## 🚀 Key Highlights
✅ End-to-end pipeline with train-test split and CV  
✅ Comparison of multiple boosting frameworks  
✅ Feature importance, SHAP, and residual analysis  
✅ Metrics: MAE, RMSE, R², and Adjusted R²  

---

## 📊 Model Results
### Prediction Scatter
![Prediction vs Actual](./Gradient%20Boosted%20Regression%20Trees/pred_vs_actual_gbrt.png)

### Residual Analysis
![Residual Plot](./Gradient%20Boosted%20Regression%20Trees/residual_plot_gbrt.png)

### Feature Importance
![Feature Importance](./Gradient%20Boosted%20Regression%20Trees/feature_importance_gbrt.png)

---

## 💡 Insights
- Gradient boosting models outperform traditional regressors.
- Feature-level interpretability available via SHAP.
- CatBoost provides superior handling of categorical data.

---


---

# 📉 Linear Regression

The **Linear Regression** model estimates the relationship between dependent and independent variables by minimizing squared errors.

---

## 🚀 Key Highlights
✅ Includes baseline regression metrics and diagnostics  
✅ Normality, heteroscedasticity, and residual tests  
✅ Coefficient interpretation and feature importance  

---

## 📊 Model Results
### Predicted vs Actual
![Predicted vs Actual](./Linear%20Regression/predicted_vs_actual.png)

### Residual Analysis
![Residuals](./Linear%20Regression/residual_plot.png)

### Feature Coefficients
![Coefficients](./Linear%20Regression/coefficients.png)

---

## 💡 Insights
- Ideal baseline for benchmarking other regressors.
- Performs well on linearly separable continuous targets.
- Residual plots indicate minimal bias and constant variance.

---


---

# 🧠 Neural Networks (for continuous outputs)

A deep learning approach using **Keras/TensorFlow**, capturing complex non-linear relationships between inputs and outputs.

---

## 🚀 Key Highlights
✅ Uses dense feed-forward architecture  
✅ Loss functions: MSE & MAE  
✅ Early stopping and dropout regularization  
✅ Performance visualization with learning curves  

---

## 📊 Model Results
### Learning Curve
![Learning Curve](./Neural%20Networks%20(for%20continuous%20outputs)/learning_curve_nn.png)

### Loss Curve
![Loss Curve](./Neural%20Networks%20(for%20continuous%20outputs)/loss_curve_nn.png)

### Prediction Scatter
![Prediction vs Actual](./Neural%20Networks%20(for%20continuous%20outputs)/prediction_vs_actual_nn.png)

---

## 💡 Insights
- Outperforms simpler regressors on complex datasets.
- Dropout effectively prevents overfitting.
- Best for capturing nonlinear dependencies.

---

---

# 📊 Polynomial Regression

Extends Linear Regression by fitting polynomial features of input variables, capturing curvature and nonlinear patterns.

---

## 🚀 Key Highlights
✅ Pipeline: Polynomial feature expansion + Linear model  
✅ Includes MAE, RMSE, R², and residual analysis  
✅ Comparison of degree-based fits  

---

## 📊 Model Results
### Polynomial Fit (Degree 2 vs 3)
![Polynomial Fit](./Polynomial%20Regression/polynomial_fit_comparison.png)

### Residual Plot
![Residual Plot](./Polynomial%20Regression/residual_plot_poly.png)

### Learning Curve
![Learning Curve](./Polynomial%20Regression/learning_curve_poly.png)

---

## 💡 Insights
- Performs best with moderate degree (2–3).  
- High degrees risk overfitting; validated via CV.  
- Demonstrates non-linear flexibility with interpretability.

---


---

# 🧩 Ridge, Lasso & ElasticNet Regression

Regularized linear models addressing overfitting and multicollinearity.  
Each method applies different penalties to control coefficient magnitude.

---

## 🚀 Key Highlights
✅ Ridge (L2), Lasso (L1), ElasticNet (L1+L2) implemented  
✅ CV-based alpha tuning with metrics comparison  
✅ Feature selection visualization for Lasso  

---

## 📊 Model Results
### Feature Importance
![Feature Importance](./Ridge_lasso/feature_importance_ridge.png)

### Coefficient Paths
![Coefficient Paths](./Ridge_lasso/coef_path_lasso.png)

### Residual Plot
![Residual Plot](./Ridge_lasso/residual_plot_ridge.png)

---

## 💡 Insights
- **Ridge:** Stabilizes coefficients for correlated features.  
- **Lasso:** Performs feature selection via shrinkage.  
- **ElasticNet:** Balances both penalties for hybrid control.  

---

## 👨‍💻 Author
**Shubham Singh**

---

## 📜 License
MIT License
