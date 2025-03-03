# oibsib_task1
# Title: house price prediction using linear regression 
# Project Overview
This project aims to predict house prices using Linear Regression based on various features like area, number of bedrooms, bathrooms, parking space, and more. The dataset was cleaned, analyzed, and used to train a predictive model to estimate house prices accurately.

# **Dataset**: 
![image alt](https://github.com/Harjibola051/oibsib_task1/blob/main/18.png?raw=true)

The dataset contains 545 rows and 13 columns with various features related to houses, including:

**Numerical Features**: Price, area, bedrooms, bathrooms, stories, parking

**Categorical Features (Encoded)** : Mainroad access, guestroom, basement, air conditioning, hot water heating, preferred area, furnishing status

# 1. Data Exploration & Preprocessing
Checked for missing values and data types


Analyzed skewness and outliers in numerical features using histograms, boxplots, and statistical tests

Applied Interquartile Range (IQR) method to remove outliers in price and area. 

# 2. Feature Engineering
- Converted categorical variables into numerical format using one-hot encoding

- Checked for multicollinearity using Variance Inflation Factor (VIF) and a correlation heatmap

- Used Lasso Regression and Random Forest Feature Importance to select the most significant features

# 3. Model Training & Evaluation
- Split data into training (80%) and testing (20%) sets
- Standardized features using StandardScaler

# Trained a Linear Regression model
# Results:
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R-squared (R²) Score

- 
# 4. Model Interpretation & Visualization
- Plotted actual vs predicted house prices
- Analyzed residual distribution to check assumptions of linear regression
- Used Q-Q plots and scatter plots to assess error distribution


# Results & Insights
The model provides a reasonable approximation of house prices, with an R² score indicating the percentage of variance explained
Outlier removal and feature selection significantly improved accuracy
Future improvements could include non-linear models (e.g., Random Forest, XGBoost) for better performance

# Technologies Used
- Python (pandas, numpy, seaborn, matplotlib, sklearn, statsmodels)
- Machine Learning: Linear Regression, Lasso Regression, Random Forest
- Data Visualization: Correlation heatmaps, histograms, boxplots, residual plots
