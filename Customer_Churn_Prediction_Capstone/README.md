# Customer Churn Prediction Using Logistic Regression From Scratch

This project predicts whether a telecom customer is likely to churn using **Logistic Regression implemented from scratch with NumPy**.

The main purpose of this project was not only to build a churn prediction model, but also to understand how Logistic Regression works internally.

## Problem Statement

Customer churn occurs when a customer stops using a company's services.

The goal of this project is to identify customers who are more likely to churn so that the company can take retention actions before losing them.

## Dataset

The project uses the **Telco Customer Churn Dataset**.

- Total Customers: 7,043
- Original Columns: 21
- Target Variable: `Churn`

The dataset contains customer information such as:

- Tenure
- Contract Type
- Monthly Charges
- Total Charges
- Internet Service
- Payment Method
- Tech Support
- Online Security
- Other Services

## Project Workflow

1. Data Understanding
2. Exploratory Data Analysis (EDA)
3. Data Cleaning
4. Feature Engineering
5. Encoding
6. Train-Test Split
7. Feature Scaling
8. Handling Class Imbalance
9. Logistic Regression From Scratch
10. Model Training
11. Model Evaluation
12. Scikit-Learn Comparison
13. Business Insights

## Data Preprocessing

Important preprocessing steps include:

- Removed the `customerID` column
- Converted `TotalCharges` to numeric format
- Handled missing values
- Created a new `Total_Services` feature
- Applied Binary Encoding
- Applied One-Hot Encoding
- Used Standard Scaling
- Used an 80/20 train-test split

## Handling Class Imbalance

The dataset contains more non-churn customers than churn customers.

To handle this imbalance, I used **class weights** so that churn customers receive more importance during model training.

## Logistic Regression From Scratch

Instead of only using a pre-built Machine Learning model, I implemented Logistic Regression from scratch using **NumPy**.

The implementation includes:

- Sigmoid Function
- Binary Cross-Entropy / Log Loss
- Class-Weighted Loss
- Gradient Descent
- Weight and Bias Updates
- Probability Prediction
- Binary Classification

The model was trained for **2,000 iterations** with a learning rate of **0.1**.

## Model Performance

### Custom Logistic Regression

| Metric | Score |
| --- | ---: |
| Accuracy | 74.10% |
| Precision | 50.78% |
| Recall | 78.34% |
| F1 Score | 61.62% |
| ROC-AUC | 84.01% |

### Scikit-Learn Logistic Regression

| Metric | Score |
| --- | ---: |
| Accuracy | 73.88% |
| Precision | 50.52% |
| Recall | 78.34% |
| F1 Score | 61.43% |
| ROC-AUC | 84.15% |

Both models produced very similar results, which helped validate the custom implementation.

## Key Insights

From the Exploratory Data Analysis:

- Month-to-month contract customers showed higher churn.
- Customers with shorter tenure showed higher churn.
- Fiber optic customers had relatively higher churn.
- Customers without Tech Support showed higher churn.
- Customers without Online Security showed higher churn.
- Electronic Check users showed higher churn.

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-Learn
- Google Colab / Jupyter Notebook

## Project Structure

Customer_Churn_Prediction_Capstone/
- Data/
  - WA_Fn-UseC_-Telco-Customer-Churn.csv
- Churn_Prediction.ipynb
- Customer_Churn_Prediction_Capstone_Report.pdf
- README.md

## What I Learned

Through this project, I gained practical experience with:

- Exploratory Data Analysis
- Data Cleaning and Preprocessing
- Feature Engineering
- Handling Class Imbalance
- Logistic Regression
- Sigmoid Function
- Gradient Descent
- Model Evaluation
- Comparing a custom model with Scikit-Learn

Most importantly, this project helped me understand how **Logistic Regression works internally**, instead of only using it through a Machine Learning library.

## Future Improvements

The project can be improved further by:

- Testing different classification thresholds
- Performing additional feature engineering
- Using cross-validation
- Comparing with other classification algorithms
- Deploying the model as a web application

## Author

**Krishna Kumawat**

BTech Computer Science & Engineering  
JECRC University