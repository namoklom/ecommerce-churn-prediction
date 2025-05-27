# Customer Churn Prediction in E-Commerce Company

## 👤 Author

| Name            | Role              | LinkedIn                                      |
|-----------------|-------------------|-----------------------------------------------|
| Jason Emmanuel  | Data Scientist | [linkedin.com/in/jasoneml](https://www.linkedin.com/in/jasoneml/) |

## 🚀 Project Overview
This project focuses on predicting customer churn for one of Indonesia's largest e-commerce startups. By leveraging advanced data analytics and machine learning techniques, the goal is to build a predictive tool that anticipates whether a customer will remain loyal or churn. This enables the company to implement targeted retention strategies, optimize resources, and enhance overall customer satisfaction.

## 🎯 Motivation
Instead of waiting for customers to leave, the model helps proactively engage potentially churning customers with personalized offers or recommendations. It also helps maintain stock and service quality for loyal customers, ultimately driving business growth in a competitive market.

## 📊 Dataset
The dataset contains 5630 customer records with 20 features, including demographic information, app usage patterns, transaction history, and satisfaction scores.

### 📝 Sample Features:
- `CustomerID`
- `Churn` (target variable)
- `Tenure`
- `PreferredLoginDevice`
- `CityTier`
- `PreferredPaymentMode`
- `HourSpendOnApp`
- `OrderCount`
- `CouponUsed`
- `CashbackAmount`
- … and more

## 🛠️ Project Steps

### 1. Exploratory Data Analysis (EDA) and Visualization
- Investigated data distribution, missing values, feature correlations, and categorical/numerical variable distributions.
- Key insights include class imbalance (more non-churn customers), device preferences, and correlations between order counts and device registrations.

### 2. Data Preprocessing
- Handled missing values with median imputation for numerical features and mode imputation for categorical features.
- Encoded categorical variables using one-hot encoding.
- Scaled numerical features for improved model performance.

### 3. Feature Engineering
- Created relevant features that help capture customer behavior patterns.
- Selected important features based on domain knowledge and correlation analysis.

### 4. Model Building
- Split data into training and testing sets.
- Developed classification models (e.g., Logistic Regression, Random Forest, or other algorithms) to predict churn.
- Tuned hyperparameters to optimize model accuracy and robustness.

### 5. Model Evaluation
- Evaluated using metrics such as accuracy, precision, recall, F1-score, and AUC-ROC.
- Analyzed confusion matrix and feature importance to interpret model results.

## 🛠️ Tools & Libraries

| Tool / Library               | Description                                                                 |
|-----------------------------|-----------------------------------------------------------------------------|
| Python                      | Core language for building the churn prediction pipeline                    |
| pandas, numpy               | Data manipulation and numerical operations                                  |
| matplotlib, seaborn, plotly | Data exploration and graphical representation                               |
| scikit-learn, imblearn      | Preprocessing, encoding, scaling, and handling class imbalance              |
| scikit-learn (models)       | Machine learning models (e.g., Logistic Regression, Random Forest, etc.)    |
| scikit-learn.metrics        | Model evaluation using accuracy, precision, recall, F1-score, ROC-AUC       |

## ▶️ How to Run
Clone the repository:
   ```bash
   git clone https://github.com/yourusername/ecommerce-churn-prediction.git
