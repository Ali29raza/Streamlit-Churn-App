# Customer Churn Prediction App

## Project Overview
This project aims to build a machine learning model that predicts customer churn for a telecommunications company based on various features such as tenure, internet service type, contract type, and charges. By utilizing these features, the model provides insights into factors influencing customer retention.

## Dataset
**Telco Customer Churn Dataset**

### Features:
- **tenure**: Number of months the customer has been with the company.
- **InternetService**: Type of internet service (DSL, Fiber optic, No).
- **Contract**: Type of contract (Month-to-month, One year, Two year).
- **MonthlyCharges**: Monthly charges for the service.
- **TotalCharges**: Total charges incurred by the customer.
- **Churn**: Binary label indicating whether the customer has churned (1) or not (0).

## Model
For this project, the following machine learning models were considered:

- Logistic Regression
- Random Forest
- Support Vector Machine (SVM)
- AdaBoost
- XGBoost

Each model's performance was evaluated based on:

- Accuracy
- Feature importance

Hyperparameters were fine-tuned to optimize prediction accuracy where applicable.

## Data Preprocessing
Missing values were handled by filling in appropriate values, and categorical features were encoded into numerical values.

## Results
The final models yielded the following results:

- **Best Model**: Random Forest
- **Best Accuracy**: 81%
- **Key Features**:
  - Monthly contract
  - Total charges
  - Tenure

These features significantly influenced customer churn rates, providing insights into factors that affect customer retention.

## Streamlit App
The project includes a user-friendly **Streamlit app** that allows users to input customer data and predict the likelihood of churn. The app features:

- **Input Fields**: Users can enter details such as tenure, internet service type, contract type, monthly charges, and total charges.
- **Prediction Result**: After entering the information, users can toggle to make a prediction, which indicates whether the customer is likely to stay or churn.
- **Visual Feedback**: The app provides visual feedback, including celebratory balloons for retained customers and error messages for those likely to churn.


## Installation and Requirements
To run the project locally, you will need to have the following Python libraries installed:

- pandas
- numpy
- scikit-learn
- xgboost
- joblib 
- streamlit

## Future Improvements
- Experiment with more advanced models, such as deep learning (ANN).
- Explore additional feature engineering techniques to enhance prediction accuracy.
- Improve the Streamlit app's UI/UX for better user engagement.
