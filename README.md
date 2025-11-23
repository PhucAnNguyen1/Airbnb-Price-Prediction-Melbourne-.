# Airbnb-Price-Prediction-Melbourne-
## Overview

This project focuses on building a complete machine learning workflow to predict Airbnb listing prices in Melbourne using a publicly available Kaggle dataset. The dataset contains detailed information on host characteristics, property features, amenities, location coordinates, availability, and review history. The objective is to prepare the data, explore it visually, engineer predictive features, train regression models, and evaluate their performance.
The final output includes a fully functional predictive model and insights into the factors that most strongly influence Airbnb prices.

## Project Objectives

Predict the price of an Airbnb listing using structured and semi-structured data.
Explore key drivers of listing price across property, host, and location characteristics.
Apply best practices in data cleaning, preprocessing, and feature engineering.
Compare multiple machine learning regression models.
Tune model hyperparameters and select the best-performing model.

1. Data Understanding:
- Loaded the Airbnb dataset and inspected its structure, data types, missing values, and descriptive statistics.
- Identified inconsistencies, extreme outliers, duplicate records, and noisy text fields.

3. Data Cleaning:
- Removed or imputed missing values depending on variable type.
- Treated outliers using IQR thresholds and domain knowledge.
- Standardised or normalised numerical features where needed.
- Encoded categorical features using one-hot, ordinal, and frequency encoding approaches.

4. Feature Engineering: 
- Parsed the amenities text field into binary indicator features.
- Engineered location-based variables, such as distance to Melbourne CBD and neighbourhood encodings.
- Created property-level metrics such as:
  - price per guest
  - host experience length
  - review frequency and review scoring ratios
- Generated correlation heatmaps and feature-importance plots to inform model choices.

5. Modelling: 
Trained and compared several regression models:
- Linear Regression
- Ridge Regression
- Lasso Regression
- Random Forest Regressor
- XGBoost Regressor
- Split the dataset into training and test sets.
- Tuned hyperparameters using GridSearchCV and RandomizedSearchCV.

6. Evaluation: 
Evaluated models using:

- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)
- R² score
- Selected the best-performing model (typically Random Forest or XGBoost depending on tuned results).
- Interpreted model behaviour and identified the strongest predictors of Airbnb prices.

7. Final Deliverables
- A cleaned and transformed dataset ready for modelling.
- A trained regression model with competitive performance.
- A price prediction CSV file formatted for Kaggle submission.
- Full analysis notebook with EDA, feature engineering, modelling, and evaluation.

8. Tools and Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Jupyter Notebook
