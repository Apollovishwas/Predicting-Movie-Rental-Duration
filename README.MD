# DVD Rental Duration Prediction

## Project Overview

This project aims to develop a regression model that predicts the number of days a customer will rent a DVD based on various features. The goal is to achieve a Mean Squared Error (MSE) of 3 or less on a test set, helping the DVD rental company improve their inventory planning efficiency.

## Dataset

The dataset `rental_info.csv` contains the following features:

- `rental_date`: Date and time of DVD rental
- `return_date`: Date and time of DVD return
- `amount`: Amount paid for the rental
- `amount_2`: Square of the amount
- `rental_rate`: Rate at which the DVD is rented
- `rental_rate_2`: Square of the rental rate
- `release_year`: Year the movie was released
- `length`: Length of the movie in minutes
- `length_2`: Square of the movie length
- `replacement_cost`: Cost to replace the DVD
- `special_features`: Additional features on the DVD
- `NC-17`, `PG`, `PG-13`, `R`: Dummy variables for movie ratings

## Methodology

1. **Data Preprocessing**:
   - Handle missing values
   - Convert date columns to appropriate format
   - Calculate rental duration (target variable)

2. **Exploratory Data Analysis**:
   - Visualize relationships between features and rental duration
   - Identify correlations and potential feature importance

3. **Feature Engineering**:
   - Create new features if necessary (e.g., day of week, month)
   - Handle categorical variables (e.g., special_features)

4. **Model Development**:
   - Split data into training and testing sets
   - Train multiple regression models (e.g., Linear Regression, Random Forest, Gradient Boosting)
   - Perform hyperparameter tuning

5. **Model Evaluation**:
   - Use Mean Squared Error (MSE) as the primary metric
   - Conduct cross-validation for robustness

6. **Model Selection**:
   - Choose the model that achieves MSE ≤ 3 on the test set

## Tools Used

- Python
- Pandas for data manipulation
- Scikit-learn for model development and evaluation
- Matplotlib/Seaborn for data visualization