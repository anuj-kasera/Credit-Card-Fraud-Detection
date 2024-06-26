# Credit-Card-Fraud-Detection

<h2>Dataset</h2>
The dataset used for this project was extracted from Kaggle. It has a total of 2,84,807 transactions, out of which 492 are fraudulent. Therefore, the dataset is highly imbalanced.

<h2>Data Preprocessing</h2>

1. Loading the Dataset: Read the dataset using pandas and inspected its structure.

2. Exploratory Data Analysis: Explored data distribution, checked for missing values, and visualized class distributions.

3. Data Balancing: Applied different techniques:
   i) SMOTE (Synthetic Minority Over-sampling Technique): Oversampled the minority class to balance the dataset.
   ii) RandomOversampler()
   iii) RandomUndersampler()

4. Feature Scaling: Standardized numerical features using StandardScaler.

<h2>Model Building</h2>

1. Baseline Models: Trained Logistic Regression, Decision Tree, and Random Forest classifiers.

2. Hyperparameter Tuning: Used GridSearchCV to optimize hyperparameters for models.

3. Model Evaluation: Evaluated models using ROC AUC score, confusion matrix, accuracy, sensitivity, specificity, and F1-score.

<h2> Results and Conclusion</h2>

XGBoost with SMOTE emerged as the top performer:

<b> ROC AUC score:</b> 0.9999 (train), 0.9833 (test).
<br>Decision was made to avoid undersampling due to potential information loss.

Conclusion: Based on its simplicity, efficiency, and outstanding performance metrics, XGBoost with SMOTE is recommended as the best model for credit card fraud detection in this scenario.
