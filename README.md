# House Prices Prediction

This repository contains a machine learning project aimed at predicting house prices using various regression models. The project involves data preprocessing, feature selection, data visualization, and model evaluation to identify the best regression model for predicting house prices.

## Dataset

The dataset consists of two files:
- `train.csv`: 1460 rows and 81 columns
- `test.csv`: 1459 rows and 80 columns

## Project Workflow

1. **Data Concatenation**
   - Combine the train and test datasets for preprocessing.

2. **Missing Values Handling**
   - Identify and handle missing values.
   - Fill missing values with the mean for numerical columns and the most common value for categorical columns.

3. **Feature Selection**
   - Use mutual information regression to identify important features for predicting house prices.

4. **Data Visualization**
   - Analyze the price distribution with histograms and boxplots.
   - Examine the relationship between price and overall house quality using boxplots.
   - Perform bivariate analysis to explore relationships between price and other columns.

5. **Correlation Analysis**
   - Check the correlation between columns to identify potential multicollinearity.

6. **Model Building and Evaluation**
   - Train and evaluate the following regression models using Grid Search:
     - Linear Regression
     - Random Forest
     - Ridge Regression
     - Decision Tree
     - XGBoost
     - CatBoost

## Data Visualization

- **Price Distribution**
  - Histogram and boxplot to visualize the distribution of house prices.
- **Price vs. Overall House Quality**
  - Boxplot to visualize the relationship between house prices and overall quality.
- **Bivariate Analysis**
  - Various visualizations to explore the relationship between house prices and other features.

## Correlation Analysis

- Compute the correlation matrix to identify highly correlated features and potential multicollinearity.

## Feature Selection

- Use mutual information regression to select the most important features for predicting house prices.

## Model Evaluation

- Train and evaluate various regression models.
- Use Grid Search for hyperparameter tuning.
- The CatBoost model with Grid Search achieved the best performance with a 91% prediction accuracy, as measured by Root Mean Squared Error (RMSE).

## Results

The CatBoost regression model outperformed all other models with the highest prediction accuracy of 91%.

## Repository Structure

