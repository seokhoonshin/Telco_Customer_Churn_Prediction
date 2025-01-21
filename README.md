# Telco Customer Churn Prediction: BA305_Final_Project

## Overview
This project focuses on predicting customer churn in the telecom industry using machine learning. By identifying key drivers of churn and implementing targeted retention strategies, the project aims to enhance customer satisfaction and reduce churn rates.

---

## Key Features
- **Dataset:**
  - Telco Customer Churn dataset with 21 features and 7,043 observations.
- **Target:**
  - Predict whether a customer will churn (Yes/No).
- **Techniques:**
  - Addressed class imbalance using **SMOTE**.
  - Applied hyperparameter tuning for **Random Forest**, **XGBoost**, **CatBoost**, and **LightGBM** models.
  - Evaluated feature importance to identify key churn drivers.

---

## Methodology

### Data Preprocessing
- Encoded categorical variables and converted binary responses to numerical values.
- Removed multicollinear features (e.g., dropped `TotalCharges` due to high correlation with `tenure`).

### Exploratory Data Analysis (EDA)
- Identified high churn rates among:
  - Month-to-month contract customers.
  - Customers using electronic check as a payment method.
- Found `tenure` and `monthly charges` as significant predictors of churn.

### Model Development
- **Logistic Regression (Baseline):**
  - Accuracy: 81%
  - F1-Score: 0.81
- **Random Forest:**
  - Accuracy: 85%
  - F1-Score: 0.85 (Recommended for deployment)
- **LightGBM:**
  - Accuracy: 84%
  - F1-Score: 0.84 (Ideal for real-time applications)

---

## Results

### Key Insights
- **High churn drivers:**
  - Month-to-month contracts.
  - Electronic check payment methods.
  - Short tenure and higher monthly charges.

### Model Performance
- **Random Forest** and **LightGBM** demonstrated robust performance with minimal overfitting.

---

## Recommendations
1. Promote longer-term contracts to reduce churn risk.
2. Offer alternative payment options for electronic check users.
3. Design personalized retention strategies for high-risk customers:
   - Short tenure.
   - High monthly charges.

---

## Future Directions
- Incorporate real-time customer data and external datasets for enhanced predictions.
- Explore advanced algorithms, including deep learning, for identifying complex patterns in larger datasets.

---

## Tools and Technologies
- **Programming Language:** Python
- **Libraries and Frameworks:** Scikit-learn, LightGBM, XGBoost, CatBoost, Pandas, NumPy
- **Data Visualization:** Matplotlib, Seaborn

---

## How to Use
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/telco-churn-prediction.git
