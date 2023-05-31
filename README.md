**Soccer Player Market Value Prediction**
This repository contains Python scripts that focus on predicting the market value of soccer players based on various metrics. We use both statistical models and machine learning models to predict the market value.

**Main Files and Functions**
**read_and_preprocess_data**: This function reads the dataset from a CSV file, preprocesses it by normalizing and scaling the feature variables, and then returns the feature and target variables.

**Mutual_information_score**: This function calculates and prints the mutual information scores for each feature with respect to the target variable, which represents the dependency of two variables.

**pearson**: This function calculates the Pearson and Spearman correlation coefficients for all features with respect to the target variable.

**plot_coefficients**: This function plots the scatterplot of each feature against the market value. These plots help to visually understand the relationship between each feature and the target variable.

**implementOLSLinearRegression**: This function fits an Ordinary Least Squares (OLS) regression model to the data, predicts the market value for the test data, and prints the coefficients of each feature. It also calculates and prints the Mean Squared Error (MSE) and R-squared score of the model.

**predict_from_neural_network**: This function fits a simple neural network to the data, predicts the market value for the test data, and prints the MSE. It also calculates and prints the feature importance by averaging the absolute weights of the first layer of the neural network.

**shap_permutation_importance**: This function uses SHAP and permutation importance methods to interpret the predictions of a neural network model. It prints the mean and standard deviation of permutation importance for each feature.

**How to use**
Import the necessary libraries.

Use the read_and_preprocess_data function to get the preprocessed data.

Use the Mutual_information_score, pearson, and plot_coefficients functions for exploratory data analysis.

Use the implementOLSLinearRegression function to fit an OLS regression model and evaluate its performance.

Use the predict_from_neural_network function to fit and interpret a simple neural network model.

Use the shap_permutation_importance function to interpret the predictions of a neural network model using SHAP and permutation importance.

**Requirements**
The following Python packages are required: pandas, sklearn, statsmodels, matplotlib, seaborn, keras, numpy, shap.

**Note**
Some functions assume that you have the actual market values for the test data. Make sure to replace 'actual_values' with the actual Series of market values in your dataset.

Please note that the data used in these scripts is not included in this repository due to privacy concerns. You need to replace '/content/drive/MyDrive/Player_Soccer_work/data/transformed_data.csv' with the path to your own dataset.
