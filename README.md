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
- [Contributors](#contributors)
- [Usage](#usage)



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

## Screenshots

Here’s a screenshot of the application:

![prediction page](https://github.com/chandrashekhard17/forest-fires-prediction-algerian-dataset/blob/main/screenshots/Screenshot%20(189).png)


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
3. Running the Application
    ```bash
    python application.py
    ```

## Contributors
- [Chandrashekhar D](https://github.com/chandrashekhard17)

## Usage
The usage of a forest fire prediction model, like the one you're developing with the Algerian forest fires dataset, can have significant benefits for various stakeholders. Here are some potential applications:

1. **Early Warning Systems**: The model can be integrated into early warning systems to alert local authorities and communities about the likelihood of forest fires, allowing for timely preventive measures.

2. **Resource Allocation**: Governments and organizations can use the predictions to allocate firefighting resources more effectively. By understanding which areas are at higher risk, they can pre-position equipment and personnel.

3. **Land Management**: Forest managers can use the predictions to implement better land management practices, such as controlled burns or clearing brush in areas most at risk, to reduce the potential for larger fires.

4. **Public Awareness Campaigns**: The model can help inform public awareness campaigns about fire safety and prevention, particularly during high-risk periods.

5. **Insurance and Risk Assessment**: Insurance companies can use the predictions to assess risk and set premiums for properties in fire-prone areas.

6. **Research and Policy Making**: Researchers can use the data and predictions to study the impact of climate change and other factors on forest fires, helping policymakers to create more effective environmental regulations and disaster response plans.

7. **Environmental Conservation**: Conservation organizations can use the model to identify vulnerable ecosystems and prioritize conservation efforts in areas at risk of fire.

8. **Community Preparedness**: Local communities can use the predictions to develop and practice emergency response plans, enhancing their preparedness for potential fires.

Incorporating your model into a web application, as you plan with Flask, can make these predictions easily accessible to users, providing a user-friendly interface for inputting data and receiving predictions. This can enhance the model's impact and usability in real-world scenarios.


