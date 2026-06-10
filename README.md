Heart Disease Predictor  jff

Overview

This project focuses on predicting the presence of heart disease using machine learning techniques. Multiple models, including Logistic Regression, Support Vector Machines (SVM), Decision Trees, Random Forest, and XGBoost, were built and evaluated to identify the best-performing approach for accurate heart disease prediction.

Dataset

The dataset used in this project is the Cleveland Heart Disease dataset, containing medical records of 920 patients described by 14 key features. These features include demographic details (age, sex), clinical measurements (resting blood pressure, cholesterol levels), electrocardiographic results, and angiographic factors. The target variable indicates the presence (1) or absence (0) of heart disease, making this a binary classification task.

Key Features:

age: Age of the patient in years
sex: Gender (0 = male, 1 = female)
cp: Chest pain type (0-3)
trestbps: Resting blood pressure (mm Hg)
chol: Serum cholesterol (mg/dl)
fbs: Fasting blood sugar > 120 mg/dl (1 = true, 0 = false)
restecg: Resting electrocardiographic results (0-2)
thalach: Maximum heart rate achieved
exang: Exercise-induced angina (1 = yes, 0 = no)
oldpeak: ST depression induced by exercise
slope: Slope of the peak exercise ST segment (0-2)
ca: Number of major vessels colored by fluoroscopy (0-4)
thal: Thalium stress test result (0-3)
num: Heart disease status (0 = no, 1 = yes)
Key Steps

Data Exploration & Cleaning
Explored summary statistics, handled missing values, and fixed structural inconsistencies.

Imputation & Encoding
Applied median/mode imputation, KNN and iterative imputation for missing values; used One-Hot, Ordinal, and Label encoding for categorical variables.

Outlier Detection
Checked for outliers; minimal presence of outliers was retained since models like Random Forest, SVM, and XGBoost are robust to them.

Modeling
Built baseline models: Logistic Regression, SVM, Decision Tree, Random Forest, and XGBoost.
Performed hyperparameter tuning using both Grid Search CV and Bayesian Optimization.
Additionally, tuned model decision thresholds to optimize performance metrics.

Evaluation
Assessed models using accuracy, precision, recall, and confusion matrix analysis.

Ensembling
Combined multiple models into an ensemble to further improve accuracy, achieving a final accuracy of 85.3%.

Results

The ensemble model demonstrated strong predictive performance with an accuracy of 85.3% and balanced precision and recall, indicating its effectiveness in detecting heart disease cases accurately.

How to Run

Requirements

Make sure to install the following libraries before running the code:

Usage

Clone the repository:

Open the notebook:

Open HEART_DISEASE_PREDICTOR.ipynb in Jupyter Notebook or VS Code.
Run all cells sequentially to perform the full data exploration, preprocessing, modeling, and evaluation pipeline.
Author

Sagar Jassar
