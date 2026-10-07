  
🛒 E-commerce Customer Churn Prediction

A Machine Learning project that predicts whether an e-commerce customer is likely to churn (stop using the service) based on their purchasing behavior, customer details, and interaction history.

📌 Project Overview

Customer churn is an important problem for e-commerce businesses because retaining existing customers is often more valuable than acquiring new ones.

This project uses customer behavior data to build a Machine Learning classification model that predicts customer churn and identifies the factors that have the most influence on customer retention.

The project includes data preprocessing, exploratory data analysis, visualization, model training, prediction, and evaluation.

🎯 Objectives

- Predict whether a customer is likely to churn.
- Analyze customer behavior and purchasing patterns.
- Identify important factors related to customer churn.
- Build and evaluate a Machine Learning classification model.

📊 Dataset

The dataset contains 2,000 customer records with information related to customer demographics, purchasing activity, and engagement.

Important Features

Feature| Description
"customer_id"| Unique customer identifier
"country"| Customer's country
"age"| Customer's age
"gender"| Customer's gender
"tenure_months"| Duration of customer relationship
"avg_order_value"| Average value of customer orders
"orders_last_12m"| Number of orders in the last 12 months
"returns_last_12m"| Number of returns in the last 12 months
"support_tickets"| Number of customer support tickets
"preferred_channel"| Customer's preferred communication channel
"device"| Device used by the customer
"discount_rate"| Discount usage rate
"last_purchase_days"| Days since the customer's last purchase
"signup_year"| Year the customer signed up
"churn"| Target variable indicating whether the customer churned

Target Variable

- "0" → Customer did not churn
- "1" → Customer churned

🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

🔄 Project Workflow

Dataset
   ↓
Data Cleaning
   ↓
Data Preprocessing
   ↓
Exploratory Data Analysis
   ↓
Data Visualization
   ↓
Train-Test Split
   ↓
Random Forest Classifier
   ↓
Prediction
   ↓
Model Evaluation
   ↓
Feature Importance Analysis

🔍 Exploratory Data Analysis

Different customer characteristics were analyzed to understand their relationship with churn.

The analysis included:

- Age
- Gender
- Customer tenure
- Average order value
- Number of orders
- Number of returns
- Support tickets
- Discount rate
- Days since last purchase

Visualizations were created using Matplotlib to compare customer behavior between churned and non-churned customers.

🤖 Machine Learning Model

A Random Forest Classifier was used to predict customer churn.

from sklearn.ensemble import RandomForestClassifier

model = RandomForestClassifier(random_state=42)
model.fit(X_train, y_train)

y_pred = model.predict(X_test)

The dataset was divided into:

- 80% Training Data
- 20% Testing Data

📈 Model Evaluation

The model was evaluated using:

- Accuracy
- Confusion Matrix
- Classification Report

The model achieved approximately 79% accuracy on the test dataset.

«Note: Since the dataset has fewer churned customers than non-churned customers, accuracy alone is not sufficient to judge the model. The confusion matrix and classification report were also considered.»

⭐ Feature Importance

The Random Forest model helped identify the features that contributed most to its predictions.

Some of the important features were:

1. Average Order Value
2. Discount Rate
3. Last Purchase Days
4. Tenure Months
5. Age
6. Orders in Last 12 Months

This analysis helps understand which customer behaviors may be associated with churn.

💡 Key Insights

- Customer purchasing behavior plays an important role in churn prediction.
- Last purchase activity can provide useful information about customer engagement.
- Average order value and discount rate were among the more influential features in the model.
- Customer tenure and order frequency also contributed to the prediction.

📁 Project Structure

E-commerce-Customer-Churn-Prediction/
│
├── dataset/
│   └── ecommerce_customer_churn.csv
│
├── notebooks/
│   └── customer_churn_prediction.ipynb
│
├── README.md
│
└── requirements.txt

🚀 How to Run the Project

1. Clone the repository

git clone YOUR_GITHUB_REPOSITORY_LINK

2. Open the project folder

cd E-commerce-Customer-Churn-Prediction

3. Install the required libraries

pip install pandas numpy matplotlib scikit-learn jupyter

4. Start Jupyter Notebook

jupyter notebook

Open the project notebook and run the cells step by step.

📌 Future Improvements

- Handle class imbalance using techniques such as SMOTE or class weighting.
- Compare Random Forest with other classification algorithms.
- Improve recall for the churn class.
- Perform hyperparameter tuning.
- Build an interactive dashboard for churn analysis.
- Deploy the model as a web application.

👩‍💻 Author

Urvi Agarwal

B.Tech – Artificial Intelligence & Data Science

Project

E-commerce Customer Churn Prediction Model

---

⭐ If you find this project useful, consider giving the repository a star!