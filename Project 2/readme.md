# Fraud Detection Pipeline using Supervised Machine Learning

## Project Overview
This project implements an end-to-end **Fraud Detection Pipeline** using supervised machine learning techniques. The objective is to identify fraudulent financial transactions in a highly imbalanced dataset by applying data preprocessing, handling class imbalance, training multiple classification models, hyperparameter tuning, and evaluating performance using appropriate metrics.

## 🎯 Project Objectives
- Detect fraudulent financial transactions using supervised learning.
- Handle class imbalance using **SMOTE (Synthetic Minority Over-sampling Technique)**.
- Train and compare multiple machine learning algorithms(Logistic Regression, Random Forest) .
- Evaluate models using metrics suitable for imbalanced datasets.
- Identify the best-performing model for fraud detection.


## 📂 Dataset
- **Dataset:** PaySim - Synthetic Financial Dataset for Fraud Detection
- **Sample Size:** 200,000 transactions
- **Target Variable:** `isFraud`

The dataset contains transaction details such as:
- Transaction Type
- Transaction Amount
- Sender and Receiver Balances
- Fraud Labels

## 🛠 Technologies & Libraries Used
- **Programming Language:** Python
- **Development Environment:** Jupyter Notebook
- **Data Manipulation:** Pandas, NumPy
- **Data Visualization:** Matplotlib, Seaborn
- **Machine Learning:** Scikit-learn (Logistic Regression, Random Forest, StandardScaler, GridSearchCV, RandomizedSearchCV)
- **Imbalanced Data Handling:** Imbalanced-learn (SMOTE)

## 📊 Project Workflow
- Data Loading
- Data Understanding and Exploratory Data Analysis (EDA)
- Data Cleaning & Feature Selection
- One-Hot Encoding
- Train-Test Split
- Handling Class Imbalance using SMOTE
- Feature Scaling using StandardScaler
- Logistic Regression Model
- Random Forest Model
- Hyperparameter Tuning
- Model Evaluation & Comparison
- Final Model Selection

## 🤖 Models Implemented
- Logistic Regression
- Tuned Logistic Regression
- Random Forest
- Tuned Random Forest

## 📈 Evaluation Metrics
Since the dataset is highly imbalanced, model performance was evaluated using:
- Precision
- Recall
- F1-Score
- ROC-AUC
- Accuracy (for reference only)

## 🏆 Model Performance
| Model | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|--------|---------:|----------:|--------:|---------:|--------:|
| Logistic Regression | 96.06% | 2.96% | 92.31% | 5.75% | 0.9740 |
| Tuned Logistic Regression | 96.60% | 3.48% | 94.23% | 6.71% | 0.9758 |
| **Random Forest** | **99.91%** | **63.49%** | **76.92%** | **69.57%** | **0.9988** |
| Tuned Random Forest | 99.91% | 61.54% | 76.92% | 68.38% | 0.9989 |

## ✅ Final Model
The **Random Forest Classifier** was selected as the final model because it achieved the best overall balance between:
- Precision
- Recall
- F1-Score
- ROC-AUC
Although the tuned Random Forest achieved a marginally higher ROC-AUC score, the default Random Forest produced better Precision and F1-Score, making it the preferred model for fraud detection.

## 👨‍💻 Author
**Ashish Kumar Sen**  
Data Science Intern at Decode Labs