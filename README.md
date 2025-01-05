# Telco_Customer_Churn_Prediction
BA305_Final_Project

**Customer Churn Prediction in the Telecom Industry**

This project focuses on predicting customer churn in the telecom industry using machine learning, enabling targeted retention strategies and enhancing customer satisfaction.

**Key Features**

Dataset: The Telco Customer Churn dataset with 21 features and 7043 observations.

Target: Predict whether a customer will churn (Yes/No).

Techniques:
Addressed class imbalance using SMOTE.
Applied hyperparameter tuning for Random Forest, XGBoost, CatBoost, and LightGBM models.
Evaluated feature importance to identify key churn drivers.

**Methodology**

Data Preprocessing:
Encoded categorical variables and converted binary responses to numerical values.
Removed multicollinear features (e.g., dropped TotalCharges due to high correlation with tenure).

Exploratory Data Analysis:
Identified high churn rates among month-to-month contract customers and electronic check users.
Found tenure and monthly charges as significant churn predictors.

Model Development:
Logistic Regression (baseline): Accuracy 81%, F1-score 0.81.
Random Forest: Accuracy 85%, F1-score 0.85 (recommended for deployment).
LightGBM: Accuracy 84%, F1-score 0.84 (ideal for real-time applications).

**Results**

Key Insights:
Month-to-month contracts and electronic check payments strongly correlate with churn.
Short tenure and higher monthly charges increase churn likelihood.

Model Performance:
Random Forest and LightGBM demonstrated robust performance with minimal overfitting.

**Recommendations**

Promote longer-term contracts to reduce churn risk.
Offer alternative payment options for electronic check users.
Design personalized retention strategies for high-risk customers (short tenure, high charges).

**Future Directions**

Incorporate real-time customer data and external datasets for enhanced predictions.
Explore advanced algorithms, including deep learning, for complex patterns in larger datasets.
