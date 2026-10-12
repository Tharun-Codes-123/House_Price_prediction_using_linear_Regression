# House Price Prediction Using Linear Regression

## Project Overview

This project builds a machine learning regression model to predict median house values using the California housing dataset. It explores relationships between housing characteristics and property values, preprocesses the data, and implements Linear Regression from scratch using Gradient Descent.

## Objectives

- Explore the dataset and understand the distribution of housing features.
- Identify and handle missing values without introducing data leakage.
- Analyze outliers and correlations between numerical features.
- Encode categorical variables using one-hot encoding.
- Standardize input features using StandardScaler.
- Implement Linear Regression from scratch using NumPy.
- Evaluate model performance using regression metrics and visualizations.

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Workflow

1. **Data Loading and Exploration:** Loaded the California housing dataset and examined its structure, data types, and descriptive statistics.
2. **Train-Test Split:** Divided the dataset into training and testing sets using an 80:20 split.
3. **Missing-Value Handling:** Imputed missing values in the `total_bedrooms` column using the training-set mean.
4. **Exploratory Data Analysis:** Used boxplots, histograms, and a correlation heatmap to examine feature distributions, outliers, and relationships.
5. **Categorical Encoding:** Applied one-hot encoding to the `ocean_proximity` feature and aligned the training and testing columns.
6. **Feature Scaling:** Standardized the input features using StandardScaler, fitting it only on the training data.
7. **Model Implementation:** Built a custom Linear Regression model using a cost function, gradient calculations, and iterative Gradient Descent updates.
8. **Prediction and Evaluation:** Generated predictions on the test set and evaluated them using MAE, MSE, RMSE, and R².
9. **Visualization:** Plotted actual versus predicted house values to examine prediction performance.

## Model Implemented

**Linear Regression from Scratch**

The model uses Gradient Descent to optimize its weights and bias by minimizing the squared-error cost function.

- Learning rate: 0.01
- Training iterations: 5,000
- Optimization: Batch Gradient Descent

## Evaluation Metrics

- **MAE (Mean Absolute Error):** Measures the average absolute prediction error.
- **MSE (Mean Squared Error):** Measures the average squared prediction error.
- **RMSE (Root Mean Squared Error):** Expresses prediction error in the target variable's units.
- **R² Score:** Measures how much of the variation in the target is explained by the model.

## Key Learning Outcomes

- Understanding the complete workflow of a regression problem.
- Implementing Linear Regression and Gradient Descent without relying on a ready-made regression estimator.
- Preventing data leakage during preprocessing.
- Understanding the importance of feature scaling and categorical encoding.
- Evaluating regression models using numerical metrics and visual analysis.

## Future Improvements

- Compare the custom implementation against Scikit-learn's LinearRegression.
- Experiment with Ridge and Lasso Regression.
- Tune the learning rate and number of iterations.
- Explore feature engineering and additional regression models.
- Analyze residuals to identify systematic prediction errors.
