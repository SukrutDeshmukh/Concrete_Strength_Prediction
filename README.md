# Concrete_Strength_Prediction

![GettyImages-941748918-5c7f3654c9e77c00012f82f6](https://github.com/SukrutDeshmukh/Concrete_Strength_Prediction/assets/127339353/0b6903a1-bf02-4cee-97fc-3382b3bb3131)

# Basic Information related to the project 
 
1) Concrete is a composite material made up of fine and coarse aggregates combined with cement paste, which solidifies and strengthens over time.
2) Cement is a crucial component in the preparation of concrete, contributing approximately 22% to the composition.
3) India holds the position of the second-largest cement producer globally, with a share of over 7% of the total installed capacity.
4) In FY 2022, the domestic production of cement in India reached 356 million tons, indicating a growth from 296 million tons in FY 2021.


# Project Information

The main goal of this project is to thoroughly examine a given dataset and apply various machine learning models to it. The dataset contains information about the composition of concrete, and the ultimate objective is to predict the strength of the concrete based on the provided composition data. The project aims to evaluate different machine learning models and determine the most suitable model that yields accurate predictions for the dataset.

# Dataset Features Information

1) Cement: The amount of cement (in kg/m³) used in the concrete mixture.
2) Slag: The amount of slag (in kg/m³) included in the concrete mixture.
3) Flyash: The quantity of fly ash (in kg/m³) incorporated in the concrete mixture.
4) Water: The volume of water (in kg/m³) used during the preparation of concrete.
5) Superplasticizer: The amount of superplasticizer (in kg/m³) added to improve the workability of the concrete.
6) Coarse Aggregate: The proportion of coarse aggregate (in kg/m³) used in the concrete mixture. This typically consists of gravel or crushed stone.
7) Fine Aggregate: The proportion of fine aggregate (in kg/m³) used in the concrete mixture. This usually refers to sand.
8) Age: The age of the concrete sample (in days) at the time of testing for strength.
9) csMPa: The compressive strength of the concrete sample (in MPa), which is the target variable to be predicted.

These features provide crucial information about the composition and age of the concrete samples, and the target variable (csMPa) represents the measured compressive strength of the concrete.

# Steps Performed in the project

1) Checked for null values and any noises present in the dataset.
2) Examined the data types of each feature and checked for duplicate data.
3) Identified the numerical and categorical features in the dataset.
4) Analyzed the age groups' trends using a histogram.
5) Explored the relationships between different features using a pair plot.
6) Used a heatmap to identify the features that are closely related to the target variable.
7) Conducted an analysis of outliers in the dataset.
8) Performed a train-test split to divide the dataset into training and testing sets.
9) Created a linear regression model using the data and evaluated its performance.
10) Created a decision tree model using the data and evaluated its performance.
11) Created a random forest model using the data and evaluated its performance.
12) Performed hyperparameter tuning using random search CV.
13) Created a support vector regression (SVR) model using the data and evaluated its performance.
14) Applied grid search CV for further hyperparameter tuning.
15) Implemented polynomial linear regression for 2nd and 3rd-degree polynomial features.

# Data Visuals & Model Comparsion

a) Analyzed the kernel density function (KDF) to visualize the distribution and estimate the probability density of the data.

![Screenshot (694)](https://github.com/SukrutDeshmukh/Concrete_Strength_Prediction/assets/127339353/482aae74-6e5e-49bc-bee7-f9da0176374b)

Examined the kernel density function (KDF) to compare the distributions with real compositions used in concrete and observed a close similarity between the data and the real compositions.

![image](https://github.com/SukrutDeshmukh/Concrete_Strength_Prediction/assets/127339353/a50107bc-8818-4d28-bf45-94e3426a3c0c)


b) Plotted Correlation heatmap to understand the other feature relation with the target.

![Screenshot (696)](https://github.com/SukrutDeshmukh/Concrete_Strength_Prediction/assets/127339353/96d89fc7-9a3e-49f6-9746-413bdb950512)

Observed that cement shares a good relationship with the target.

c) Different Machine Learning Model R2 Evaluations score comparison.

The R2 score measures how well a regression model fits the data. It ranges from 0 to 1, where 0 indicates no relationship and 1 indicates a perfect fit. Higher R2 scores indicate a better fit of the model to the data, suggesting that the independent variables are effective in predicting the target variable. However, it should be used alongside other metrics to evaluate the model's overall performance.

![Screenshot (697)](https://github.com/SukrutDeshmukh/Concrete_Strength_Prediction/assets/127339353/bcac56b2-0409-491d-82db-a237e3070d38)

Random forest scored better compared to the other models.

d) Comparsion between Random Forest & Random Forest(with Grid search Cv)

Grid Search CV is a technique used to systematically search for the best combination of hyperparameters for a machine learning model. It performs cross-validation on all possible combinations of hyperparameters specified in a grid and selects the combination that achieves the best performance. It helps automate the process of hyperparameter tuning and improves the model's performance by finding the optimal hyperparameters.

![Screenshot (698)](https://github.com/SukrutDeshmukh/Concrete_Strength_Prediction/assets/127339353/7e78dd11-ccf3-46fc-80b2-37f82d685e02)

e) Polynomial Degree (1, 2, 3) 

![Screenshot (702)](https://github.com/SukrutDeshmukh/Concrete_Strength_Prediction/assets/127339353/c9d6d7dc-74d8-49b2-b724-9a5bde7c39e9)

When we increased the polynomial degree in polynomial regression, we observed a decrease in the spread between the predicted values and the actual data points. This indicated that the model was better capturing the underlying patterns in the data. The increased flexibility of the higher degree polynomial allowed the model to fit the data more closely.

f) All the model's comparison visuals.

![Screenshot (703)](https://github.com/SukrutDeshmukh/Concrete_Strength_Prediction/assets/127339353/eeaf385c-19ba-4285-a98f-7714be1cf376)

Conclusion: Random forest is the best-suited model for the dataset.










