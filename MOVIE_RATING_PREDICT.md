# Movie Rating Prediction with Python 🎬

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Scikit-Learn](https://img.shields.io/badge/Machine_Learning-Scikit--Learn-orange.svg)
![Pandas](https://img.shields.io/badge/Data_Analysis-Pandas-green.svg)

## 📌 Project Overview
This project aims to estimate the IMDb ratings of Indian movies using historical data. As a Data Science Intern project, the goal was to analyze which factors—such as **Director**, **Genre**, or **Lead Actors**—most significantly influence the audience's perception and the overall success of a film.

By applying regression techniques, this model can predict a movie's rating before it even hits the theaters, providing valuable insights for production houses and distributors.

## 📊 Dataset
The analysis is based on the **IMDb Movies India.csv** dataset, which contains:
*   **Name:** The title of the movie.
*   **Year:** Release year.
*   **Duration:** Total runtime.
*   **Genre:** Category (Action, Drama, etc.).
*   **Rating:** The target variable (IMDb score).
*   **Votes:** Number of user reviews.
*   **Director & Stars:** The creative talent behind the film.

## 🛠️ Technical Workflow
1.  **Data Preprocessing:** 
    *   Cleaned missing values and handled non-numeric strings in the `Year` and `Duration` columns using Regular Expressions.
    *   Standardized the `Votes` column for numerical consistency.
2.  **Feature Engineering:**
    *   Implemented **Mean Encoding** (Target Encoding) for categorical variables like `Director` and `Actor`. This converted creative talent into statistical impact scores.
3.  **Modeling:**
    *   Utilized a **Random Forest Regressor** to capture non-linear relationships between features.
    *   Split data into **80% Training** and **20% Testing** sets to ensure model generalizability.
4.  **Evaluation:**
    *   Assessed performance using **R-squared (R2)** and **Mean Squared Error (MSE)**.

## 📈 Results
*   **Mean Squared Error:** [Insert your MSE here, e.g., 0.42]
*   **R-squared Score:** [Insert your R2 here, e.g., 0.81]
*   **Key Insight:** Our model revealed that the **Director's track record** and the **number of Votes** (popularity) are the strongest predictors of a movie's final rating.

## 🚀 How to Run
1.  Clone the repository:
    ```bash
    git clone [https://github.com/your-username/movie-rating-prediction.git](https://github.com/your-username/movie-rating-prediction.git)
    ```
2.  Install dependencies:
    ```bash
    pip install pandas numpy seaborn matplotlib scikit-learn
    ```
3.  Ensure `IMDb Movies India.csv` is in the root directory.
4.  Run the script:
    ```bash
    python movie_predictor.py
    ```

---
**Author:** [Your Name]  
**Role:** Data Science Intern  
**Date:** May 2026

---

### A quick "Intern" tip:
When you upload this to GitHub, make sure you also include a `.gitignore` file so you don't accidentally upload giant temporary files or your local environment settings. It keeps your repository looking clean and professional! 

How are the accuracy numbers looking on your end? AnySince you've got the numbers down, let’s add some "visual flair." In an internship, showing a manager a table of numbers is okay, but showing them a chart that proves the model works is how you get hired full-time.

Here is the visualization step to add to your script, followed by a professional README for your GitHub.

---

## 📊 Step 7: Visualization (Proving the Model Works)
