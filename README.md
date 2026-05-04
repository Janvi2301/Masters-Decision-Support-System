# 🎓 Masters Decision Support System

## 🚀 Project Overview

The **Masters Decision Support System** is a Machine Learning-based web application built using Streamlit.  
It helps students decide whether they should pursue a **Master’s degree** based on two key factors:

- 📊 GATE Score  
- 💰 Current Salary  

The system uses a trained **Random Forest Classifier** to analyze patterns from historical data and provide a recommendation.

---

## 🎯 Objective

Many students are confused about whether to pursue higher education or continue working.  
This project aims to:

- Provide **data-driven guidance**
- Reduce decision uncertainty
- Demonstrate how Machine Learning can support real-life decisions

---

## 🧠 Why This Prediction Model?

The decision to pursue a Master’s degree depends on multiple factors.  
This model simplifies the decision using two important indicators:

### 1. GATE Score
- A higher GATE score increases chances of:
  - Admission into top institutes
  - Scholarships and financial support
- A lower score may reduce academic opportunities

### 2. Current Salary
- Higher salary → Less incentive to leave job for studies  
- Lower salary → Higher motivation to upskill through a Master’s  

---

## 🤖 Model Explanation

### Model Used:
**Random Forest Classifier**

### Why Random Forest?
- Handles both numerical and categorical data effectively  
- Reduces overfitting using multiple decision trees  
- Provides better accuracy compared to a single decision tree  
- Works well with small to medium datasets  

---

## ⚙️ How the Model Works

1. The dataset is loaded from `dataset.csv`
2. Data preprocessing is applied:
   - Categorical values (like Yes/No) are converted into numeric form
3. Features and target are defined:
   - Features → `GATE_Score`, `Salary`
   - Target → `Should_Do_Masters`
4. Dataset is split:
   - 80% for training
   - 20% for testing
5. Model is trained using Random Forest
6. Predictions are made based on user input

---

## 🔍 How Prediction is Made

When a user enters:
- GATE Score  
- Salary  

The model:
1. Compares input with learned patterns from dataset  
2. Passes input through multiple decision trees  
3. Each tree gives a vote (Yes/No)  
4. Final decision is based on **majority voting**

---

## 📊 Example Logic Behind Prediction

- ✅ High GATE Score + Low Salary  
  → Recommendation: **Do Master's**  
  → Reason: Strong academic opportunity + need for growth  

- ❌ Low GATE Score + High Salary  
  → Recommendation: **Do Not Do Master's**  
  → Reason: Weak academic opportunity + stable income  

- ⚖️ Medium values  
  → Model decides based on learned patterns  

---

## ✨ Features

- 🏠 Home Page  
- 📘 About Model (accuracy + explanation)  
- 📁 Dataset Preview  
- 🤖 Prediction System  
- 📊 Graph Visualization  

---

## 🛠️ Technologies Used

- Python  
- Streamlit  
- Pandas  
- Matplotlib  
- Scikit-learn  
- streamlit-option-menu  

---

## 📂 Project Structure
Masters-Decision-System/
│── app.py
│── dataset.csv
│── requirements.txt
│── README.md
