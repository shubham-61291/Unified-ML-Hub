# 📈 Regression (Continuous Output) — All Models Overview

A unified collection of **supervised regression models** implemented by **Shubham Singh**, covering Linear, Non-linear, and Ensemble-based approaches.  
Each model folder includes complete pipelines — from preprocessing and training to visualization and explainability.

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
Implemented using **LightGBM (GPU)** on the California Housing dataset.

---

## 🚀 Key Highlights
✅ Early stopping and hyperparameter optimization  
✅ RandomizedSearchCV + GridSearchCV tuning  
✅ Full diagnostics: MSE, RMSE, MAE, R², Adjusted R²  
✅ Feature importance, PDP/ICE, and SHAP explainability  

---

## 📈 Learning Curves
![Learning Curve - Early Stop](https://github.com/shubham-61291/Unified-ML-Hub/blob/main/supervised/Regression%20(Continuous%20Output)/Gradient%20Boosted%20Regression%20Trees/learningcurve.png?raw=true)
![Learning Curve - Random Search](https://github.com/shubham-61291/Unified-ML-Hub/blob/main/supervised/Regression%20(Continuous%20Output)/Gradient%20Boosted%20Regression%20Trees/learningcurveRSmodel.png?raw=true)
![Learning Curve - Grid Search](https://github.com/shubham-61291/Unified-ML-Hub/blob/main/supervised/Regression%20(Continuous%20Output)/Gradient%20Boosted%20Regression%20Trees/leaarningcurve_bestgridmodel.png?raw=true)

---

## 📉 Residual Diagnostics
![Validation Residuals](https://github.com/shubham-61291/Unified-ML-Hub/blob/main/supervised/Regression%20(Continuous%20Output)/Gradient%20Boosted%20Regression%20Trees/residual_validationbest.png?raw=true)
![Test Residuals](https://github.com/shubham-61291/Unified-ML-Hub/blob/main/supervised/Regression%20(Continuous%20Output)/Gradient%20Boosted%20Regression%20Trees/residual_testbest.png?raw=true)

---

## 🔍 Prediction Fit
![Validation Fit](https://github.com/shubham-61291/Unified-ML-Hub/blob/main/supervised/Regression%20(Continuous%20Output)/Gradient%20Boosted%20Regression%20Trees/actualvspredicted_validationbest.png?raw=true)
![Test Fit](https://github.com/shubham-61291/Unified-ML-Hub/blob/main/supervised/Regression%20(Continuous%20Output)/Gradient%20Boosted%20Regression%20Trees/actualvspredicted_testbest.png?raw=true)

---

## 🌿 Feature Importance & Explainability
![Top Features](https://github.com/shubham-61291/Unified-ML-Hub/blob/main/supervised/Regression%20(Continuous%20Output)/Gradient%20Boosted%20Regression%20Trees/top2features.png?raw=true)
![PDP + ICE](https://github.com/shubham-61291/Unified-ML-Hub/blob/main/supervised/Regression%20(Continuous%20Output)/Gradient%20Boosted%20Regression%20Trees/pdp_ice_bestgrid_topfeatures.png?raw=true)
![SHAP Global](https://github.com/shubham-61291/Unified-ML-Hub/blob/main/supervised/Regression%20(Continuous%20Output)/Gradient%20Boosted%20Regression%20Trees/SHAPvalue.png?raw=true)
![Local SHAP](https://github.com/shubham-61291/Unified-ML-Hub/blob/main/supervised/Regression%20(Continuous%20Output)/Gradient%20Boosted%20Regression%20Trees/localshaptest.png?raw=true)

---

## 💡 Insights
- Early stopping stabilized training near 1871 trees.  
- Median income & house age dominate predictive contribution.  
- Grid refinement achieved best R² ≈ 0.86.

---

---

# 📉 Linear Regression

Performs a classic **Ordinary Least Squares** regression on the California Housing dataset, benchmarking model simplicity and interpretability.

---

## 🚀 Key Features
✅ Automated pipeline using Scikit-learn  
✅ Multiple evaluation metrics (MSE, RMSE, MAE, R²)  
✅ Residual and prediction distribution visualization  

---

## 📊 Visual Results
![Metric Comparison](https://github.com/shubham-61291/Unified-ML-Hub/blob/main/supervised/Regression%20(Continuous%20Output)/Linear%20Regression/metric%20comparison.png?raw=true)
![Predictions (Actual vs Predicted)](https://github.com/shubham-61291/Unified-ML-Hub/blob/main/supervised/Regression%20(Continuous%20Output)/Linear%20Regression/predictions.png?raw=true)
![Residuals](https://github.com/shubham-61291/Unified-ML-Hub/blob/main/supervised/Regression%20(Continuous%20Output)/Linear%20Regression/residuals.png?raw=true)
![Residual Distribution](https://github.com/shubham-61291/Unified-ML-Hub/blob/main/supervised/Regression%20(Continuous%20Output)/Linear%20Regression/residual%20distribution.png?raw=true)

---

## 💡 Insights
- Strong linear baseline with R² ≈ 0.60  
- Residuals centered around 0 — unbiased model  
- Low variance, interpretable coefficients

---


---

# 🧠 Neural Networks (for continuous outputs)

Implements **Deep Neural Network Regression** using TensorFlow/Keras with MC Dropout and Heteroscedastic modeling for uncertainty estimation.

---

## 🚀 Key Highlights
✅ Epistemic + Aleatoric uncertainty modeling  
✅ GPU + mixed precision training  
✅ Visual diagnostics: Loss, Residuals, and Prediction Fit  

---

## 📈 Training Dynamics
![Loss Curve (MC Dropout)](https://github.com/shubham-61291/Unified-ML-Hub/blob/main/supervised/Regression%20(Continuous%20Output)/Neural%20Networks%20(for%20continuous%20outputs)/LosscurveMCdropout.png?raw=true)
![Learning Rate Schedule](https://github.com/shubham-61291/Unified-ML-Hub/blob/main/supervised/Regression%20(Continuous%20Output)/Neural%20Networks%20(for%20continuous%20outputs)/LRscheduleMCdropout.png?raw=true)

---

## 📉 Residual Diagnostics
![Residual Validation](https://github.com/shubham-61291/Unified-ML-Hub/blob/main/supervised/Regression%20(Continuous%20Output)/Neural%20Networks%20(for%20continuous%20outputs)/residual_validation.png?raw=true)
![Residual Test](https://github.com/shubham-61291/Unified-ML-Hub/blob/main/supervised/Regression%20(Continuous%20Output)/Neural%20Networks%20(for%20continuous%20outputs)/residual_test.png?raw=true)

---

## 🔍 Prediction Fit
![Validation Fit](https://github.com/shubham-61291/Unified-ML-Hub/blob/main/supervised/Regression%20(Continuous%20Output)/Neural%20Networks%20(for%20continuous%20outputs)/actualvspredicted_validation.png?raw=true)
![Test Fit](https://github.com/shubham-61291/Unified-ML-Hub/blob/main/supervised/Regression%20(Continuous%20Output)/Neural%20Networks%20(for%20continuous%20outputs)/actualvspredicted_test.png?raw=true)

---

## 💡 Insights
- MC Dropout captures epistemic uncertainty effectively.  
- Heteroscedastic NN improves aleatoric variance modeling.  
- Smooth loss curves indicate stable convergence.

---


---

# 📊 Polynomial Regression

Extends linear regression by fitting polynomial relationships between median income and housing prices.

---

## 🚀 Key Highlights
✅ Polynomial degree 1–4 comparison  
✅ Adjusted R² used for degree selection  
✅ Evaluation across validation, test, and CV splits  

---

## 📈 Visual Results
![MSE Comparison](https://github.com/shubham-61291/Unified-ML-Hub/blob/main/supervised/Regression%20(Continuous%20Output)/Polynomial%20Regression/MSE.png?raw=true)
![R² Comparison](https://github.com/shubham-61291/Unified-ML-Hub/blob/main/supervised/Regression%20(Continuous%20Output)/Polynomial%20Regression/R2.png?raw=true)
![Learning Curve](https://github.com/shubham-61291/Unified-ML-Hub/blob/main/supervised/Regression%20(Continuous%20Output)/Polynomial%20Regression/learning%20curve.png?raw=true)
![Residual Distribution](https://github.com/shubham-61291/Unified-ML-Hub/blob/main/supervised/Regression%20(Continuous%20Output)/Polynomial%20Regression/residual%20distribution.png?raw=true)

---

## 💡 Insights
- Degree 4 polynomial achieved best generalization.  
- Captures mild nonlinearity while avoiding overfitting.  
- Ideal for moderate feature–target curvatures.

---


---

# 🧩 Ridge, Lasso & ElasticNet Regression

Regularized linear regressors controlling overfitting and multicollinearity using L1 and L2 penalties.

---

## 🚀 Key Highlights
✅ Ridge, Lasso & ElasticNet with α tuning  
✅ Coefficient path visualization  
✅ ElasticNet heatmap and residual comparison  

---

## 📈 Visual Results
![R² Comparison](https://github.com/shubham-61291/Unified-ML-Hub/blob/main/supervised/Regression%20(Continuous%20Output)/Ridge_lasso/R2%20comparison.png?raw=true)
![RMSE Comparison](https://github.com/shubham-61291/Unified-ML-Hub/blob/main/supervised/Regression%20(Continuous%20Output)/Ridge_lasso/RMSE%20comparison.png?raw=true)
![Coefficient Paths](https://github.com/shubham-61291/Unified-ML-Hub/blob/main/supervised/Regression%20(Continuous%20Output)/Ridge_lasso/Coefficientpaths_LASSO.png?raw=true)
![Residual Plot](https://github.com/shubham-61291/Unified-ML-Hub/blob/main/supervised/Regression%20(Continuous%20Output)/Ridge_lasso/ridge_residual.png?raw=true)
![Feature Importance Ridge](https://github.com/shubham-61291/Unified-ML-Hub/blob/main/supervised/Regression%20(Continuous%20Output)/Ridge_lasso/feature_importance_ridge.png?raw=true)

---

## 💡 Insights
- Ridge Regression (α≈6.25) achieved optimal bias–variance balance.  
- Lasso performed automatic feature selection.  
- ElasticNet blended both regularizations effectively.

---

## 👨‍💻 Author
**Shubham Singh**

---

## 📜 License
MIT License
