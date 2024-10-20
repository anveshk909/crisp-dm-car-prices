
# **Used Car Price Analysis**

## **Overview**
This project explores a dataset containing information about 426,000 used cars. The goal is to analyze which factors influence car prices, helping a used car dealership fine-tune its pricing and inventory strategies. This project follows the CRISP-DM framework and utilizes machine learning models to predict car prices based on features like manufacturer, odometer readings, condition, and more.

## **Dataset**
The dataset was sourced from Kaggle and contains the following key variables:
- `price`: Selling price of the car (target variable)
- `year`: Year of manufacture
- `manufacturer`: The make of the car
- `condition`: Vehicle condition (excellent, good, etc.)
- `cylinders`: Number of engine cylinders
- `fuel`: Fuel type
- `odometer`: Mileage of the vehicle
- `drive`: Type of drive (e.g., front-wheel drive)
- `type`: Type of vehicle (e.g., sedan, SUV)

## **Project Structure**
The repository contains the following files:
- **notebook.ipynb**: The Jupyter notebook containing the complete analysis, data cleaning, EDA, and modeling.
- **README.md**: This file, summarizing the project.
- **vehicles.csv**: The dataset used for the analysis (you can include a link to it or instructions on how to download it).
  
## **CRISP-DM Framework**
The project follows the CRISP-DM process:
1. **Business Understanding**: Identify factors that affect used car prices.
2. **Data Understanding**: Explore the dataset, handle missing values, and clean the data.
3. **Data Preparation**: Encode categorical variables and prepare the data for modeling.
4. **Modeling**: Implement machine learning models, including Linear Regression and Random Forest.
5. **Evaluation**: Evaluate models using MAE and RMSE to compare performance.
6. **Deployment**: Provide insights and recommendations for the dealership.

## **Key Findings**
1. **Mileage (Odometer)**: Cars with lower mileage tend to have higher prices.
2. **Manufacturer**: Premium car brands like Audi, BMW, and Mercedes command higher prices.
3. **Condition**: Cars in excellent condition tend to have significantly higher prices.
4. **Year of Manufacture**: Newer cars generally sell for higher prices.

## **Modeling Results**
- **Linear Regression**: MAE = \$6410.75, RMSE = \$10,550.80
- **Random Forest**: MAE = \$4179.79, RMSE = \$6,892.46

The Random Forest model performs better than Linear Regression, as it captures non-linear relationships between variables.

## **Recommendations**
- Focus on acquiring low-mileage cars in excellent condition.
- Target premium brands for higher profit margins.
- Adjust pricing strategy based on mileage, brand, and condition for better customer targeting.

## **Next Steps**
- Further fine-tuning of the Random Forest model using GridSearchCV or advanced hyperparameter tuning.
- Additional feature engineering, such as including external factors like regional demand or seasonal effects, to enhance the model's predictive power.




# **Used Car Price Prediction**

## **Overview**
This project explores the factors that influence used car prices. A dataset containing 426,000 car listings is analyzed to identify key factors such as mileage, brand, condition, and more that affect car prices. Using machine learning models, including Linear Regression and Random Forest, we aim to provide predictive insights for a used car dealership.

## **CRISP-DM Framework**
This project follows the CRISP-DM framework:
1. **Business Understanding**: Understand the factors that drive car prices.
2. **Data Understanding**: Explore the dataset to identify trends and quality issues.
3. **Data Preparation**: Handle missing values, encode categorical variables, and clean the data.
4. **Modeling**: Build and evaluate machine learning models.
5. **Evaluation**: Assess model performance using metrics such as MAE and RMSE.
6. **Deployment**: Provide actionable insights for the used car dealership.

## **Key Findings**
1. **Mileage**: Lower mileage correlates with higher prices.
2. **Manufacturer**: Premium brands like Audi and BMW command higher prices.
3. **Condition**: Cars in better condition fetch significantly higher prices.
4. **Year of Manufacture**: Newer cars generally have higher prices.

## **Models Used**
- **Linear Regression**: MAE = \$6410.75, RMSE = \$10,550.80
- **Random Forest**: MAE = \$4179.79, RMSE = \$6,892.46

## **Recommendations**
- Prioritize acquiring low-mileage cars in good or excellent condition.
- Focus on premium brands for higher profitability.
- Adjust pricing strategy based on the model's insights to maximize returns.

## **Next Steps**
- Fine-tune the models further using GridSearchCV and additional features.
- Consider external factors such as demand and seasonal trends to improve predictions.

## **Instructions**
- Clone this repository and run the notebook to reproduce the analysis.
- Ensure the `vehicles.csv` dataset is available in the same directory.
