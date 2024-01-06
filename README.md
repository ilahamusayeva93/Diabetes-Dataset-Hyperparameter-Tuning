# Pima Indian Diabetes Classification 

## Overview

This case study focuses on predicting the likelihood of diabetes in individuals using the Pima Indian diabetes dataset. The dataset contains various health-related features, and an XGBoost Classifier is employed for the classification task. Hyperparameter tuning is performed using Grid Search and Randomized Search strategies to enhance model performance.

## Dataset

### Origin and Objective
The dataset originates from the National Institute of Diabetes and Digestive and Kidney Diseases. The objective is to predict whether a patient has diabetes or not based on diagnostic measurements. The dataset consists of 768 rows with 9 columns, including features such as pregnancies, glucose concentration, blood pressure, and more.

### Features
1. Pregnancies – Number of times pregnant
2. Glucose – Plasma glucose concentration 2 hours in an oral glucose tolerance test
3. BloodPressure – Diastolic blood pressure (mm Hg)
4. SkinThickness – Triceps skinfold thickness (mm)
5. Insulin – 2-Hour serum insulin (mu U/ml)
6. BMI – Body mass index (weight in kg / (height in m)^2)
7. DiabetesPedigreeFunction – Diabetes pedigree function
8. Age – Age (years)
9. Outcome – Class variable (0 or 1) indicating diabetes presence (1) or absence (0)

## Data Preprocessing

### Exploratory Data Analysis
- Examination of missing values, duplicates, and basic statistics.
- Visualization of the correlation heatmap to understand feature relationships.

### Feature Selection
- Dropping unnecessary columns.
- Splitting the data into features (X) and target variable (y).

### Data Scaling
- Scaling features using RobustScaler to handle outliers.

## Model Training

### XGBoost Classification
- Splitting the data into training and testing sets.
- Training an XGBoost Classifier on the scaled data.
- Evaluating the model's performance using accuracy metrics.

### Hyperparameter Tuning - RandomizedSearchCV
- Utilizing RandomizedSearchCV to explore hyperparameter space.
- Tuning parameters such as learning rate, number of estimators, and maximum depth.

### Hyperparameter Tuning - GridSearchCV
- Employing GridSearchCV for an exhaustive search over specified parameter values.
- Fine-tuning hyperparameters to improve model accuracy.

## Model Evaluation

- Evaluating the final model on the test set.
- Generating classification reports to assess precision, recall, and accuracy.

## Results

- Presenting the results of the tuned XGBoost Classifier.
- Comparing the outcomes of RandomizedSearchCV and GridSearchCV.

## Additional Libraries

- scikit-optimize (skopt) is used for Bayesian Optimization.
- Optuna is employed for another hyperparameter optimization approach.

## Conclusion

This case study demonstrates the application of XGBoost in diabetes classification, emphasizing the significance of hyperparameter tuning for improved model performance. The insights gained from the study contribute to understanding the factors influencing diabetes prediction.

## Author

Ilaha Musayeva
09/09/23

**Disclaimer:** The dataset used for this analysis is from the National Institute of Diabetes and Digestive and Kidney Diseases. The study aims to predict diabetes, and interpretation should be cautious.
