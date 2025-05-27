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

## 📊 Visualizations

![image](https://github.com/user-attachments/assets/7fb1d390-8186-4dfa-8a84-1a71fa9ef274)

This heatmap visualizes the Pearson correlation coefficients between relevant features in a churn prediction dataset. A value close to 1 indicates a strong positive correlation, while a value near -1 indicates a strong negative correlation. Notably, Churn is moderately negatively correlated with Tenure (-0.35), suggesting that customers with longer tenure are less likely to churn. CouponUsed and OrderCount (0.75), as well as CouponUsed and DaySinceLastOrder (0.36), show strong to moderate positive correlations, indicating potential behavioral patterns. Interestingly, CashbackAmount has a modest positive correlation with Tenure (0.48), implying loyal customers may receive more cashback. These relationships help identify influential features for churn prediction.

![image](https://github.com/user-attachments/assets/5cbea980-da50-485f-819e-9825714a8060)

This set of bar plots presents the distribution of various categorical features in the dataset. Most users prefer to log in using a Mobile Phone, and City Tier 1 dominates the customer base. The majority of users are Male, and most are Married, with a notable portion being Single. In terms of payment, Debit Cards are the most preferred mode, followed by Credit Cards, while methods like Cash on Delivery and UPI are less popular. The most common product category ordered is Laptop & Accessories, followed by Mobile Phones, whereas Others and Grocery categories see less engagement. These distributions provide insight into customer demographics, preferences, and shopping behavior.

![image](https://github.com/user-attachments/assets/cd85d387-fe09-4fbd-9212-40efe93a3357)

This graph shows the training and validation loss curves over 50 epochs. The training loss (blue line) starts very high but drops sharply within the first few epochs and then continues to decrease gradually, indicating the model is learning effectively from the training data. The validation loss (orange line) also drops quickly and stabilizes at a low value early on, suggesting good generalization to unseen data. The close alignment and consistent downward trend of both curves indicate that the model is well-fitted without signs of overfitting or underfitting.

![image](https://github.com/user-attachments/assets/a487b6be-ee39-451f-ac17-87c6e5ce96a8)

This graph shows the training and validation loss curves over 50 epochs. The training loss (blue line) starts very high but drops sharply within the first few epochs and then continues to decrease gradually, indicating the model is learning effectively from the training data. The validation loss (orange line) also drops quickly and stabilizes at a low value early on, suggesting good generalization to unseen data. The close alignment and consistent downward trend of both curves indicate that the model is well-fitted without signs of overfitting or underfitting.

![image](https://github.com/user-attachments/assets/dc9acd7c-8279-4449-a746-0c468835f603)

This graph illustrates the training and validation accuracy over 50 epochs. The training accuracy (blue line) shows a steady increase, indicating that the model is learning and fitting the training data well. However, the validation accuracy (orange line) remains flat at around 81.4%, suggesting that while the model improves on the training set, it does not generalize better to unseen data after a certain point. This gap between training and validation accuracy indicates overfitting, where the model becomes too specialized to the training data and fails to improve performance on the validation set.

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
   git clone https://github.com/namoklom/ecommerce-churn-prediction.git
