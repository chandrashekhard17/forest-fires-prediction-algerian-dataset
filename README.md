# Algerian Forest Fires Prediction

This project aims to predict fire occurrences in the forests of Algeria based on the data collected from different regions. The project involves an end-to-end machine learning pipeline using exploratory data analysis (EDA), feature engineering, regression models, and model deployment. The main objective is to estimate the occurrence of fires during specific months.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset Information](#dataset-information)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Feature Engineering](#feature-engineering)
- [Modeling](#modeling)
- [Pickle Files](#pickle-files)
- [Results](#results)
- [Screenshots](#screenshots)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Contributors](#contributors)
- [License](#license)

## Project Overview
Forest fires are a serious concern in Algeria, especially during the summer months. This project aims to predict fire occurrences based on various environmental factors like temperature, wind speed, humidity, etc. The data was analyzed, processed, and used to train regression models for fire estimation. Ridge regression provided the best results, and the model was saved as a pickle file for future use.

## Dataset Information
The dataset contains environmental data collected from multiple regions in Algeria over several months. The main features in the dataset include:
- Temperature
- Humidity
- Wind Speed
- Rainfall
- FFMC (Fine Fuel Moisture Code)
- DMC (Duff Moisture Code)
- DC (Drought Code)
- ISI (Initial Spread Index)

**Target**: Fire Estimation (Burned Area)

## Exploratory Data Analysis (EDA)
EDA was performed to understand the dataset, visualize the distribution of the features, and identify correlations between them. Key insights include:
- Seasonal trends in temperature, humidity, and wind speed.
- Correlation between the Fine Fuel Moisture Code and fire occurrence.
- Outlier detection and handling.

## Feature Engineering
Feature engineering was crucial to improving the model's performance. The following steps were taken:
- Handling missing values.
- Encoding categorical features.
- Normalizing/Standardizing features.
- Feature scaling using Standard Scaler.

## Modeling
Various regression models were trained, including:
- Linear Regression
- Ridge Regression
- Lasso Regression
- Random Forest Regressor

The Ridge Regression model was selected as the final model due to its performance and ability to handle multicollinearity. The models were evaluated based on:
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R-squared

## Pickle Files
- The final Ridge Regression model was saved as a `pickle` file for future use.
- The `Standard Scaler` used during feature scaling was also saved to ensure consistent scaling for future predictions.

## Results
The Ridge Regression model achieved the best performance, with an RMSE of `XX` and an R-squared value of `YY`. The model was able to predict fire estimation with high accuracy, especially during the critical fire-prone months.

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib/Seaborn (for visualization)
- Pickle (for model saving)
- Jupyter Notebook

## Installation
To install and run this project, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/chandrashekhard17/algerian-forest-fires-prediction.git

   ```

2. Install the requirements
    ```bash
    pip install -r requirements.txt
    ```

## Contributors
- [Chandrashekhar D](https://github.com/chandrashekhard17)


