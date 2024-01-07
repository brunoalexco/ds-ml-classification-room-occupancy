# Room Occupancy Classification Project Readme

## Introduction

Hello! In this repository you will find a project related to room occupancy predictions based on the room and date characteristics. In this readme, I will provide an overview of the project, details about the dataset, the steps taken in data processing, the various models employed, and the conclusive findings.

## Project Overview

### Dataset
The dataset consists of information related to drug prescriptions and includes the following columns:

- date
- Temperature
- Humidity
- Light
- CO2
- HumidityRatio
- Occupancy

### Objective
The primary goal of this project is to predict if an office room is occupied or not based on different attributes. I cleaned the data, preprocessed it for training my models, utilized classification models, and tuned the best-performing ones with RandomizedSearch and GridSearch.

## Project Steps

1. Exploratory Data Analysis (EDA)
2. Data Preprocessing
3. Modeling
4. Optimizing
5. Evaluation

## Model Evaluation

Evaluated each model using the following metrics:

- **Accuracy Score**
- **Classification Report:** Precision, Recall, F1-Score.

## Conclusion

After thorough evaluation, the  models achieved the following accuracy rates on testing data:

Before optimizations:
  - Decision Tree Classifier - 0.99181
  - Bagging Classifier - 0.99181
  - RandomForest - 0.99304
  - KNN - 0.99181
  - Logistic Regression - 0.98608
  - LightGBM - 0.99304
  - XGBoost - 0.99181
  - Gradient Boosting - 0.99099

After optimizations: 
  - Decision Tree Classifier - 0.98895
  - RandomForest - 0.99304

Upon reviewing the classification report, the selected model for maximizing True Positives and True Negatives is RandomFores. 

## Running the Project

To run this project on your own, follow these steps:
1. Load the dataset from the provided link.
2. Execute each cell in the notebook sequentially.
3. Make sure to install any required packages if prompted.
4. Review the results and explore visualizations in the notebook.

## Python Packages Used

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- lightgbm
- xgboost

Ensure you have these packages installed before running the notebook. You can install them using this command:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn lightgbm xgboost
