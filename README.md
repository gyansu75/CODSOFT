# Data Science Internship Projects by Gaurav Gyansu
This repository is for my Data Science Internship at Codsoft.
### email : gyansu75@gmail.com 

# 1. TITANIC SURVIVAL PREDICTION

## Project Overview
This project was developed during my Data Science Internship to predict the survival probability of passengers aboard the Titanic. Using the classic Titanic dataset, I built a machine learning pipeline that cleans messy real-world data, performs exploratory analysis, and implements a Random Forest Classifier.

## 🎯 Objective
The goal is to answer the question: “What sorts of people were more likely to survive?” using passenger data (ie. name, age, gender, socio-economic class, etc.).

## 📊 Key Insights (EDA)
During the analysis, two major factors stood out as strong predictors for survival:
- **Gender:** Female passengers had a significantly higher survival rate than male passengers.
- **Socio-Economic Class:** Passengers in 1st Class (Pclass 1) were prioritized and had much higher survival chances compared to 3rd Class.

### 1. Data Cleaning & Preprocessing
- **Missing Values:** - Filled missing `Age` values using the **Median** to maintain a central distribution.
    - Filled missing `Embarked` ports with the **Mode** (the most frequent value).
- **Feature Selection:** Dropped `PassengerId`, `Name`, `Ticket`, and `Cabin` as they contained high unique counts or excessive missing data that didn't help with general prediction.
- **Categorical Encoding:** Converted `Sex` and `Embarked` into numerical format using One-Hot Encoding to make them readable by the model.

### 2. Machine Learning Model
- **Algorithm:** Random Forest Classifier.
- **Why Random Forest?** As an intern, I chose this because it is a "Council of Experts" (multiple decision trees) that prevents the model from just memorizing the training data, leading to better predictions on new data.
- **Reproducibility:** Used `random_state=42` to ensure consistent results every time the code runs.

### 3. Model Evaluation
- **Accuracy:** ~81.01%
- **Metrics:** Used a **Confusion Matrix** to visualize where the model correctly predicted outcomes and where it made mistakes.

## Results
- **Actual Deaths:** 95 died
- **Actual Survived:** 50 survived
- **Predicted Deaths:** 10
- **Predicted Survived:** 24

## Tools and Softwares
- **Platforms:** Jupyter, Github
- **Programming languages:** Python
- **Libraries:** Matplotlib, Seaborn, Scikit-learn



