📊 E-commerce Revenue Classification (Amazon Sales Dataset)
📌 Project Overview

This project aims to analyze e-commerce sales data and build a Machine Learning classification model to predict whether an order will generate High Revenue or Low Revenue.

The project covers the complete ML workflow:

Exploratory Data Analysis (EDA)

Data Cleaning & Preprocessing

Feature Engineering

Model Training

Model Evaluation

Feature Importance Analysis

🎯 Business Problem

In e-commerce platforms, identifying high-revenue orders can help:

Optimize marketing strategies

Improve targeting campaigns

Adjust pricing & discount strategies

Focus on high-value customers

The goal is to predict whether an order's revenue will be above or below the median revenue.

🗂 Dataset Features

The dataset includes:

price

discount_percent

quantity_sold

rating

review_count

discounted_price

product_category

customer_region

payment_method

total_revenue

Target Variable:

high_rev

1 → High Revenue

0 → Low Revenue

Threshold is defined using the median of total_revenue.

🔎 Exploratory Data Analysis (EDA)

EDA included:

Distribution of Total Revenue (Histogram + KDE)

Boxplots for numerical features

Countplots for categorical features

Correlation Matrix (Heatmap)

Key insights:

Quantity sold and price strongly impact revenue.

Discount percentage affects final revenue.

Some regions and product categories perform better than others.

⚙️ Data Preprocessing

Dropped unnecessary columns (order_id, order_date, product_id)

Created target variable using median threshold

Applied One-Hot Encoding to categorical features

Train-Test Split (80%-20%)

Applied Standard Scaling (for Logistic Regression)

🤖 Models Used

Logistic Regression

Decision Tree Classifier

Random Forest Classifier

📈 Model Evaluation Metrics

Accuracy

Confusion Matrix

Classification Report (Precision, Recall, F1-Score)

ROC-AUC (for Random Forest)

Random Forest achieved the best performance overall.

🌟 Feature Importance

Feature importance analysis showed:

Quantity Sold

Discounted Price

Price

Discount Percentage

These features had the strongest impact on predicting high revenue orders.

🛠 Technologies Used

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

🚀 How to Run the Project

Clone the repository

Install required libraries:

pip install pandas numpy matplotlib seaborn scikit-learn

Run the notebook or Python script

📌 Future Improvements

Hyperparameter tuning (GridSearchCV)

Cross-validation

ROC Curve visualization

SHAP for model explainability

Deployment using Flask / FastAPI
