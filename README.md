Heart Disease Prediction System 🫀
This repository contains a comprehensive machine learning pipeline to predict the presence of heart disease. The project covers the entire data science lifecycle: from deep exploratory data analysis and feature engineering to advanced hyperparameter tuning of multiple classifiers.

🚀 Key Features
Comprehensive EDA: Univariate and bivariate analysis using Seaborn and Matplotlib.

Data Preprocessing: * Automated handling of categorical variables (One-Hot Encoding).

Outlier detection using the IQR method.

Feature transformation using Box-Cox to handle skewed distributions.

Model Comparison: Evaluates four major algorithms:

Decision Tree (DT)

Random Forest (RF)

K-Nearest Neighbors (KNN)

Support Vector Machine (SVM)

Optimization: Utilizes GridSearchCV with StratifiedKFold to maximize Recall (crucial for medical diagnosis).

📊 Dataset Overview
The dataset contains 303 entries with 14 health attributes:

Numerical: Age, Resting Blood Pressure (trestbps), Cholesterol (chol), Max Heart Rate (thalach), ST Depression (oldpeak).

Categorical: Sex, Chest Pain Type (cp), Fasting Blood Sugar (fbs), ECG results, Exercise Induced Angina, Slope, Number of vessels (ca), and Thalassemia.

Target: 1 (Heart Disease), 0 (Normal).
📈 Methodology & Results1. Data TransformationTo improve model performance, continuous features were transformed using the Box-Cox method to achieve a more Gaussian (normal) distribution.2. Hyperparameter TuningWe used a custom function tune_clf_hyperparameters to find the best settings for each model.KNN Optimal: 9 Neighbors, Manhattan Distance.SVM Optimal: Linear Kernel with $C=0.0011$.3.
