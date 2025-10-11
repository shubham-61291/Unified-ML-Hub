Linear Regression (California Housing) 📖 Overview
The Linear Regression (California Housing) project demonstrates supervised learning using a regression approach on the California Housing dataset. It compares performance across Train/Validation/Test splits and 5-Fold Cross-Validation, while visualizing residuals, predictions, and error distributions.

🚀 Key Features
✅ Regression task predicting continuous housing prices.
✅ Comparison across Validation, Test, and Cross-Validation folds.
✅ Multiple evaluation metrics: MSE, RMSE, MAE, R², Adjusted R².
✅ Rich visual analysis: residuals, predictions, and distribution plots.
✅ Fully automated Scikit-learn pipeline.

🛠 Tech Stack
Framework: Scikit-learn
Dataset: California Housing
Libraries: NumPy, Matplotlib, Seaborn, Scikit-learn
Model: LinearRegression()
Metrics: MSE, RMSE, MAE, R², Adjusted R²

📂 Project Structure
linear_regression/
│── linear_regression.py # Core model training and evaluation script
│── metric comparison.png # Validation vs Test vs CV bar plot
│── predictions.png # Actual vs predicted comparison
│── residual distribution.png # Distribution of residuals
│── residuals.png # Validation & Test residual plots
│── residuals CV 1st fold.png # Residuals for first CV fold
│── README.md # Documentation
│── requirements.txt # Dependencies

📊 Results Summary
Train/Validation/Test Split Metrics
Validation → MSE: 0.5409, RMSE: 0.7354, MAE: 0.5335, R²: 0.5848, Adjusted R²: 0.5838
Test → MSE: 0.5203, RMSE: 0.7213, MAE: 0.5210, R²: 0.6066, Adjusted R²: 0.6055
Cross-Validation (5-Fold Average)
MSE: 0.5306, RMSE: 0.7283, MAE: 0.5317, R²: 0.6014, Adjusted R²: 0.6006

🖼 Demo

🔹 Metric Comparison
<img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAA..." width="700"/>

🔹 Predictions (Actual vs Predicted)
<img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAA..." width="700"/>

🔹 Residuals (Validation & Test)
<img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAA..." width="700"/>

🔹 Residual Distribution
<img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAA..." width="700"/>

🔹 Residuals CV (1st Fold)
<img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAA..." width="700"/>

🔮 Future Enhancements
🔹 Add Polynomial Regression comparison.
🔹 Integrate Ridge and Lasso Regression for regularization.
🔹 Include feature importance visualization.
🔹 Extend to Gradient Boosting and XGBoost regression.

👨‍💻 Author
Shubham Singh

📜 License
MIT License
