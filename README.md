House Price Prediction

This project is a machine learning model that predicts house prices based on various features such as the area, number of bedrooms, number of bathrooms, floors, year built, garage availability, location, and condition. The prediction is made using a **Random Forest Regressor** and **Linear Regression**, and a user-friendly input collection system is implemented for predictions on new data.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Library](#library)
- [Usage](#usage)
- [Modeling](#modeling)
  - [Linear Regression](#linear-regression)
  - [Random Forest Regressor](#random-forest-regressor)
- [Evaluation Metrics](#evaluation-metrics)
- [Conclusion](#conclusion)

## Project Overview

The goal of this project is to build a predictive model for house prices using features such as:
- Area
- Number of Bedrooms
- Number of Bathrooms
- Number of Floors
- Year Built
- Garage Availability
- Location (Downtown, Suburban, etc.)
- Condition of the house (Excellent, Good, Fair, Poor)

The model utilizes **Linear Regression** and **Random Forest Regressor** to make predictions and provides high accuracy results.

## Dataset

The dataset contains 2000 entries of houses with the following columns:
- `Area`: Size of the house in square meters
- `Bedrooms`: Number of bedrooms
- `Bathrooms`: Number of bathrooms
- `Floors`: Number of floors
- `YearBuilt`: Year the house was built
- `Location`: Categorical data specifying the house location (Downtown, Suburban, etc.)
- `Condition`: Categorical data specifying the condition of the house
- `Garage`: Whether the house has a garage (Yes/No)
- `Price`: Target column, house price (in local currency)

## Library
Required libraries:
- Pandas
- Numpy
- Seaborn
- Matplotlib

## Usage

After installation, you can run the `house_price_prediction.py` file to:
1. Train the models (Linear Regression, Random Forest).
2. Visualize the dataset and features.
3. Predict house prices using a command-line input system for new house data.


## Modeling

### Linear Regression

A **Linear Regression** model was initially used to fit the data. The performance was evaluated using:
- **R2 Score**: `0.9968`
- **Mean Absolute Error**: `11423.98`

### Random Forest Regressor

The **Random Forest Regressor** model was then implemented to improve prediction accuracy. This model outperformed Linear Regression, with:
- **R2 Score**: `0.9998`
- **Mean Absolute Error**: `2888.05`


## Evaluation Metrics

The models are evaluated using the following metrics:
- **R2 Score**: A statistical measure that indicates how well the regression model fits the data.
- **Mean Absolute Error (MAE)**: The average of absolute errors between predicted and actual values.

## Conclusion

The Random Forest model demonstrated superior performance in predicting house prices with a high R2 score and low MAE. The application provides accurate predictions and can be further enhanced by including more advanced techniques and hyperparameter tuning.
