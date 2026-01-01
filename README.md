🚢 Titanic Survival Prediction — Machine Learning Project
📌 Project Overview

This project focuses on building an end-to-end supervised machine learning pipeline to predict passenger survival from the historic Titanic disaster.
Using real-world data from Kaggle, the project demonstrates the complete ML workflow — from data cleaning and feature engineering to model training, tuning, and evaluation.

The goal is to accurately classify whether a passenger survived (1) or did not survive (0) based on demographic and travel-related features.

🎯 Problem Statement

Given passenger information such as:

Gender

Passenger class

Age

Fare paid

Family size

👉 Predict whether the passenger survived the Titanic disaster.

This is a binary classification problem.

📂 Dataset

Source: Kaggle — Titanic: Machine Learning from Disaster

Target Variable: Survived

1 → Survived

0 → Did not survive

🧹 Data Cleaning & Preprocessing

The following preprocessing steps were performed:

Removed irrelevant columns (PassengerId, Name, Ticket)

Handled missing values:

Age filled using median

Embarked filled using mode

Dropped Cabin due to excessive missing values

Encoded categorical features:

Sex → binary encoding

Embarked → one-hot encoding

Feature engineering:

Created FamilySize

Created IsAlone feature

Ensured all features are numeric and ML-ready

🧠 Models Used

Multiple supervised learning models were explored:

Logistic Regression (baseline)

Decision Tree Classifier

Random Forest Classifier (final model)

The final model was chosen based on performance and generalization ability.

⚙️ Model Training & Tuning

Train–test split applied after full preprocessing

Hyperparameter tuning performed using GridSearchCV

Class imbalance handled using class_weight="balanced"

📊 Model Evaluation

The Random Forest model was evaluated using:

Accuracy

Confusion Matrix

Precision, Recall, and F1-score

🔹 Final Performance

Accuracy: ~81–85%

Strong precision and recall balance

Improved generalization compared to a single decision tree

🛠️ Tools & Technologies

Python

Pandas

NumPy

Scikit-learn

Jupyter Notebook
