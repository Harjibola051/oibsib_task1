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
- Checked for missing values and data types
![image alt](https://github.com/Harjibola051/oibsib_task1/blob/main/2.png?raw=true)
![image alt](https://github.com/Harjibola051/oibsib_task1/blob/main/3.png?raw=true)

- Analyzed skewness and outliers in numerical features using histograms, boxplots, and statistical tests.
  ![image alt](https://github.com/Harjibola051/oibsib_task1/blob/main/5.png?raw=true)
  ![image alt](https://github.com/Harjibola051/oibsib_task1/blob/main/6.png?raw=true)
  ![image alt](https://github.com/Harjibola051/oibsib_task1/blob/main/7.png?raw=true)
 

Applied Interquartile Range (IQR) method to remove outliers in price and area. 
 ![image alt](https://github.com/Harjibola051/oibsib_task1/blob/main/8.png?raw=true)
 ![image alt](https://github.com/Harjibola051/oibsib_task1/blob/main/9.png?raw=true)




 
# 2. Feature Engineering
- Converted categorical variables into numerical format using one-hot encoding

- Checked for multicollinearity using Variance Inflation Factor (VIF) and a correlation heatmap

- Used Lasso Regression and Random Forest Feature Importance to select the most significant features

# 3. Model Training & Evaluation
- Split data into training (80%) and testing (20%) sets
- Standardized features using StandardScaler

# Trained a Linear Regression model
# Results:
- Mean Absolute Error (MAE): 774102.15
- Mean Squared Error (MSE): 1042591273219.80
- Root Mean Squared Error (RMSE): 1021073.59
- R-squared (R²) Score:  0.67

- 
# 4. Model Interpretation & Visualization
- Plotted actual vs predicted house prices
  ![image alt](https://github.com/Harjibola051/oibsib_task1/blob/main/15.png?raw=true)
- Analyzed residual distribution to check assumptions of linear regression
  ![image alt](https://github.com/Harjibola051/oibsib_task1/blob/main/14.png?raw=true)
- Probability plot
  ![image alt](https://github.com/Harjibola051/oibsib_task1/blob/main/19.png?raw=true)


# Results & Insights
The model provides a reasonable approximation of house prices, with an R² score indicating the percentage of variance explained
Outlier removal and feature selection significantly improved accuracy
Future improvements could include non-linear models (e.g., Random Forest, XGBoost) for better performance

# Technologies Used
- Python (pandas, numpy, seaborn, matplotlib, sklearn, statsmodels)
- Machine Learning: Linear Regression, Lasso Regression, Random Forest
- Data Visualization: Correlation heatmaps, histograms, boxplots, residual plots
