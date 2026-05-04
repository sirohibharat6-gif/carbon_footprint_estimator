# 🌱 Carbon Emission Prediction Model

A machine learning project that predicts an individual's weekly carbon emissions based on various lifestyle factors. This project demonstrates a complete data science workflow, from data cleaning and analysis to model training and evaluation.

## 📊 Project Overview

**Objective:** To develop a machine learning model that predicts an individual's weekly carbon emissions using categorical and numerical data such as diet, transport, and energy efficiency.

**Algorithm:** The model uses a **Linear Regression** algorithm to predict the continuous numerical value of carbon emissions. The focus is on creating an interpretable baseline model with robust feature selection and preprocessing.

## 🔧 Technologies Used

- **Language:** `Python 3.12`
- **Libraries:**
  - `Pandas` & `NumPy` for data manipulation and numerical operations.
  - `Scikit-learn` for model training and evaluation.
  - `Matplotlib` & `Seaborn` for data visualization.

## 🎯 Key Features

- **Data Preprocessing:** The project handles both categorical and numerical data, using **one-hot encoding** to make them suitable for the linear regression model. A **log transformation** is applied to the target variable to handle its skewed distribution, a critical step for improving model performance.
- **Linear Regression Modeling:** A linear regression model is trained on the preprocessed data to establish a clear, interpretable relationship between lifestyle features and carbon emissions.
- **Performance Visualization:** The project generates insightful visualizations to justify feature selection, explain preprocessing steps, and assess the model's final performance.
- **Results Export:** The final predictions are saved to a CSV file for further analysis and reporting.

## 📈 Model Evaluation

The model's performance was evaluated on a held-out test set (20% of the original data) to ensure a realistic assessment of its predictive power on unseen data.

### Performance Metrics

- **R-squared (R²): `0.878`**
  - This indicates that the model explains approximately **87.8%** of the variability in the carbon emission data, which is a strong result for a predictive model.

- **Mean Absolute Error (MAE): `237.30`**
  - On average, the model's predictions are off by about 237.30 units of carbon emission. This provides a straightforward measure of the average prediction error.

- **Root Mean Squared Error (RMSE): `355.96`**
  - This value is a measure of the model's error, with larger errors being penalized more heavily. The fact that the RMSE is higher than the MAE suggests that the model has a few larger prediction errors for some data points.

### Actual vs. Predicted Graph

The scatter plot below visually confirms the model's strong performance. The data points are tightly clustered around the red diagonal line, which represents a perfect prediction where the predicted value equals the actual value.

[Actual vs Predicted Plot](output.png)
