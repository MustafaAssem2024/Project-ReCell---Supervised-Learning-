# Supervised Learning - Project: ReCell

## Project Overview

The used and refurbished device market has seen significant growth, projected to be worth $52.7 billion by 2023. ReCell, a startup aiming to capitalize on this market, needs an efficient pricing strategy for used mobile phones and tablets. This project develops a machine learning model to predict the prices of these devices based on their specifications, aiding ReCell in setting competitive and profitable prices.

## Business Context

Refurbished devices provide cost-effective alternatives for consumers and businesses alike. With an increasing demand for these devices, it is crucial to establish accurate pricing strategies. ReCell, a new entrant in this market, aims to predict the price of used devices by analyzing various attributes such as brand, camera quality, battery capacity, and more. The outcome of this project will directly influence ReCell's pricing strategy, ensuring it remains competitive while maximizing profits.

## Objective

The primary objective of this project is to build a linear regression model to predict the price of used and refurbished phones and tablets. The model will identify key factors that influence the price, helping ReCell in formulating a dynamic pricing strategy.

## Data Description

The dataset contains information about various attributes of used and refurbished phones and tablets, including:

- **brand_name**: Name of the manufacturing brand
- **os**: Operating system of the device
- **screen_size**: Size of the screen in cm
- **4g**: Availability of 4G
- **5g**: Availability of 5G
- **main_camera_mp**: Resolution of the rear camera in megapixels
- **selfie_camera_mp**: Resolution of the front camera in megapixels
- **int_memory**: Internal memory in GB
- **ram**: RAM in GB
- **battery**: Battery capacity in mAh
- **weight**: Weight of the device in grams
- **release_year**: Year of device release
- **days_used**: Number of days the device has been used
- **normalized_new_price**: Normalized price of a new device in euros
- **normalized_used_price**: Normalized price of the used device in euros

## Exploratory Data Analysis (EDA)

- **Distribution Analysis**: Analyzed the distribution of normalized used prices and other key features.
- **Correlation Analysis**: Identified the relationships between different features, particularly how they influence the used price.

## Data Preprocessing

- **Missing Value Treatment**: Handled missing values by imputing with medians based on grouping factors like brand and release year.
- **Feature Engineering**: Converted the release year into the age of the device to better capture its impact on price.
- **Outlier Treatment**: Detected and addressed outliers to improve model performance.
- **Encoding**: Converted categorical variables to numerical using one-hot encoding.

## Model Development

- **Linear Regression Model**: Built using the ordinary least squares (OLS) method.
- **Multicollinearity Treatment**: Addressed multicollinearity by dropping features with high variance inflation factor (VIF).
- **Model Tuning**: Refined the model by removing features with high p-values to improve model accuracy and reliability.

## Model Evaluation

- **R-squared and Adjusted R-squared**: The final model explains approximately 84% of the variance in used device prices.
- **RMSE and MAE**: The model demonstrates low root mean squared error and mean absolute error, indicating strong predictive performance.
- **Normality and Homoscedasticity**: Verified through various statistical tests, ensuring the assumptions of linear regression were met.

## Business Insights

- **Feature Importance**: Main camera quality, selfie camera quality, RAM, and weight significantly impact the price of used devices.
- **Brand Influence**: Brands like Samsung and Xiaomi were found to have a notable influence on pricing, while age negatively impacts the price.
- **Recommendations**: Focus on enhancing key features in top-selling brands to maximize resale value.

## Conclusion

The linear regression model developed in this project provides a robust tool for predicting the price of used devices, enabling ReCell to set competitive prices. With an R-squared value of 0.84, the model is both accurate and reliable, offering actionable insights that ReCell can use to optimize its pricing strategy.


---

This project is a foundation for building dynamic pricing models, helping ReCell stay competitive in the rapidly growing used device market.
