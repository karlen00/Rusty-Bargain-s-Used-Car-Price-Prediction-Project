### README for Rusty Bargain's Used Car Price Prediction Project

## Project Description

Rusty Bargain is a company specializing in buying and selling used cars. They are developing an application to attract new buyers by providing quick estimates of the market value of their cars. You have access to historical data, vehicle technical specifications, vehicle model versions, and vehicle prices. The task is to create a model that can determine the market value of a car.

Rusty Bargain is interested in:
- Prediction quality
- Prediction speed
- Training time of the model

## Project Instructions

### 1. Data Preparation
- Load and observe the data from `/datasets/car_data.csv`.

### 2. Model Training
- Train different models with various hyperparameters. You must create at least two different models, but more is better. Note that various implementations of gradient boosting do not count as different models.
- Compare the methods of gradient boosting with random forest, decision tree, and linear regression.

### 3. Model Analysis
- Analyze the speed and quality of the models.
- Use RMSE as the evaluation metric.
- Perform a sanity check using linear regression. If gradient boosting does not outperform linear regression, there may be an issue.

### 4. Libraries and Tools
- Independently study the LightGBM library and use its tools to create a gradient boosting model.
- Include linear regression for sanity check, tree-based algorithms with hyperparameter tuning (preferably random forest), LightGBM with hyperparameter tuning (try several sets), and optionally CatBoost and XGBoost with hyperparameter tuning.
- Pay attention to categorical feature encoding for simple algorithms. LightGBM and CatBoost handle this, but XGBoost requires One-Hot Encoding (OHE).
- Use specific commands to measure cell processing time in Jupyter Notebook.
- Modify only a few parameters for gradient boosting models as training can be time-consuming.

## Data Description

The dataset includes the following features:

- **DateCrawled**: Date when the profile was downloaded from the database
- **VehicleType**: Type of vehicle body
- **RegistrationYear**: Year the vehicle was registered
- **Gearbox**: Type of transmission
- **Power**: Power (hp)
- **Model**: Model of the vehicle
- **Mileage**: Distance driven (in km according to regional dataset)
- **RegistrationMonth**: Month the vehicle was registered
- **FuelType**: Type of fuel
- **Brand**: Vehicle brand
- **NotRepaired**: Whether the vehicle has been repaired previously
- **DateCreated**: Date the profile was created
- **NumberOfPictures**: Number of vehicle pictures
- **PostalCode**: Postal code of the profile owner
- **LastSeen**: Date the user was last active

Target Variable:
- **Price**: Price (in Euros)

## Steps Taken

### Data Preparation:
1. Loaded and observed the data files.
2. Ensured data cleanliness and addressed any missing values or outliers.
3. Preprocessed the data for further analysis.

### Model Development:
1. Implemented various models to predict car prices.
2. Trained and evaluated models using appropriate metrics (RMSE).
3. Compared the performance of different models.
4. Conducted hyperparameter tuning for each model.

### Model Analysis:
1. Analyzed changes in prediction quality and speed.
2. Compared the performance of gradient boosting, random forest, decision tree, and linear regression.
3. Ensured the accuracy and effectiveness of the chosen models.

## Conclusion

This project involves preparing and analyzing data from used car listings to develop predictive models for determining market prices. It includes comparing different machine learning models and evaluating their performance in terms of accuracy, speed, and training time. The results aim to provide Rusty Bargain with a reliable model to estimate the market value of cars, enhancing their application and attracting new buyers.
