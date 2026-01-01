# 🚢 Titanic Survival Prediction  
### End-to-End Machine Learning Project

> Predicting passenger survival from the historic Titanic disaster using supervised machine learning.

---

## 📌 Project Overview
This project demonstrates a **complete end-to-end machine learning pipeline** built on the **Kaggle Titanic dataset**.  
It covers everything from **data cleaning and feature engineering** to **model training, hyperparameter tuning, and evaluation**.

🎯 **Objective:**  
Classify whether a passenger **survived (1)** or **did not survive (0)** based on demographic and travel-related features.

---

## 🎯 Problem Statement
Given passenger details such as:
- 👤 Gender  
- 🎟️ Passenger Class  
- 🎂 Age  
- 💰 Fare Paid  
- 👨‍👩‍👧 Family Size  

👉 **Predict passenger survival**  
This is a **binary classification problem**.

---

## 📂 Dataset
- **Source:** Kaggle — *Titanic: Machine Learning from Disaster*
- **Target Variable:** `Survived`
  - `1` → Survived  
  - `0` → Did not survive  

---

## 🧹 Data Cleaning & Preprocessing

### 🔹 Data Cleaning
- Removed irrelevant columns: `PassengerId`, `Name`, `Ticket`
- Handled missing values:
  - `Age` → filled with **median**
  - `Embarked` → filled with **mode**
  - Dropped `Cabin` due to excessive missing values

### 🔹 Encoding
- `Sex` → Binary encoding
- `Embarked` → One-hot encoding

### 🔹 Feature Engineering
- ➕ Created `FamilySize`
- ➕ Created `IsAlone`
- ✅ Ensured all features are numeric and ML-ready

---

## 🧠 Models Explored
The following supervised learning models were implemented:
- Logistic Regression *(baseline)*
- Decision Tree Classifier
- 🌟 **Random Forest Classifier (final model)**

The final model was selected based on **performance and generalization capability**.

---

## ⚙️ Model Training & Tuning
- Train–test split applied after preprocessing
- Hyperparameter tuning using **GridSearchCV**
- Class imbalance handled using `class_weight="balanced"`

---

## 📊 Model Evaluation

The Random Forest model was evaluated using:
- Accuracy
- Confusion Matrix
- Precision
- Recall
- F1-score

### 🔹 Final Results
- ✅ **Accuracy:** ~81–85%
- ⚖️ Balanced precision and recall
- 🚀 Better generalization than a single decision tree

---

## 🛠️ Tools & Technologies
- 🐍 Python  
- 📊 Pandas, NumPy  
- 🤖 Scikit-learn  
- 📓 Jupyter Notebook  

---

## 🚀 Key Learnings
- Complete ML workflow from raw data to evaluation
- Dataset-specific data cleaning strategies
- Feature engineering for improved performance
- Proper metric selection for classification problems
- Understanding bias–variance tradeoff

---

## 🔮 Future Improvements
- Extract titles from passenger names
- Try Gradient Boosting / XGBoost
- Improve recall for minority class
- Deploy model as a web application

---

## 👨‍💻 Author
**Sudhanshu Gocher**  
Aspiring Data Scientist | Machine Learning Enthusiast

⭐ *If you found this project helpful, feel free to star the repository!*
