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
5. **Evaluation**: Evaluate models using MSE and R² to compare performance.
6. **Deployment**: Provide insights and recommendations for the dealership.

## **Key Findings**
1. **Mileage (Odometer)**: Cars with lower mileage tend to have higher prices.
2. **Manufacturer**: Premium car brands like Audi, BMW, and Mercedes command higher prices.
3. **Condition**: Cars in excellent condition tend to have significantly higher prices.
4. **Year of Manufacture**: Newer cars generally sell for higher prices.

## **Modeling Results**
- **Linear Regression**:
  - MSE: 392,759,282,734,217.25
  - R²: -0.0033
- **Random Forest**:
  - Best Params: {'model__n_estimators': 200, 'model__min_samples_split': 2, 'model__max_depth': 10}
  - MSE: 404,233,406,108,775.56
  - R²: -0.0326
- **Voting Regressor**:
  - MSE: 395,302,296,287,610.3
  - R²: -0.0098
- **Cross-Validation (Voting Regressor)**:
  - Cross-Validation R² Scores: [-0.0472, -0.0110, -0.0070]
  - Mean Cross-Validation R²: -0.0217

The models are currently not performing well, as indicated by the negative R² values and high MSE. This suggests that the models are not capturing the relationships between features and car prices effectively.

## **Recommendations**
- **Feature Engineering**: Introduce additional features such as regional demand, seasonal trends, or safety ratings, which may provide a more accurate representation of factors affecting price.
- **Data Quality**: Ensure that the data is clean and free of outliers. Consider using techniques like robust scaling or outlier removal.
- **Hyperparameter Tuning**: Perform a more thorough search for optimal hyperparameters (e.g., using **RandomizedSearchCV** or **Bayesian optimization**).
- **Advanced Models**: Experiment with other models, such as **Gradient Boosting**, **XGBoost**, or **LightGBM**, to potentially further improve the accuracy of price predictions.
- **Ensemble Methods**: Try different ensemble methods like stacking or blending, which might improve performance.

## **Next Steps**
- **Model Integration**: Integrate the Random Forest model into the dealership's inventory management system to assist in real-time price predictions based on key features such as mileage, year, and manufacturer.
- **Price Recommendation Tool**: Develop a tool that uses the model's predictions to provide recommended price ranges for cars based on their features. This can help sales teams set competitive and profitable prices.
- **Feature Expansion**: Consider adding additional features like regional demand, safety ratings, and consumer reviews to improve the model's predictive power. This could further refine the dealership's pricing strategy.
- **Monitoring and Continuous Improvement**: As new data comes in, the model should be continuously updated and retrained to ensure that it stays accurate and reflects market trends.
- **User Training**: Train the dealership staff on how to use the new tools and interpret the model's predictions. This will ensure that they can make informed decisions based on the model's output.
- **Feedback Loop**: Establish a feedback loop where the sales team can provide insights on the model's performance and suggest areas for improvement. This will help in refining the model and making it more robust over time.
