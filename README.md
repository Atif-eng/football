# ⚽ Football Player Valuation: "The Moneyball Model"

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Library](https://img.shields.io/badge/Library-Scikit--Learn-orange)
![Algorithm](https://img.shields.io/badge/Algorithm-Random_Forest-green)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 📌 Project Overview
**"Can we build a Machine Learning model to act as a Football Scout?"**

This project applies Machine Learning to the world of football (soccer) transfers. By analyzing player stats (Goals, Assists, Age, etc.), the model predicts a player's **"Fair Market Salary"**. 

The ultimate goal is to identify **Undervalued Players**—hidden gems who are performing at a high level but are paid significantly less than their predicted worth.

**Author:** Muhammad Atif

## 📂 Dataset
The dataset contains performance metrics and financial details of professional football players.
- **Target Variable:** `Salary_M_Euro` (The player's annual salary in Millions).
- **Key Features:**
  - **Performance:** `Goals`, `Assists`, `Appearances`, `Minutes_Played`.
  - **Demographics:** `Age`, `Position`, `Team`.

## 🛠 Tech Stack
- **Language:** Python
- **Data Analysis:** `pandas`, `numpy`
- **Visualization:** `matplotlib`, `seaborn`
- **Machine Learning:** `scikit-learn` (Random Forest Regressor)

## 📊 Project Workflow

### 1. Data Loading & Engineering
- Loaded the dataset and cleaned missing values.
- **Feature Engineering:** Created new metrics to better represent player impact.
- **Visualization:** Analyzed the relationship between `Goals` and `Salary` (e.g., "Do strikers always get paid more?").

### 2. Model Training
- **Algorithm:** **Random Forest Regressor**.
- **Reasoning:** Random Forest handles non-linear relationships well (e.g., a 35-year-old player might score many goals but have a lower value due to age).
- **Split:** Used `train_test_split` to keep a portion of data unseen for testing.

### 3. Evaluation
- **Metric:** R² Score (Coefficient of Determination).
- **Result:** The model achieved an **R² Score of 0.91**, indicating extremely high accuracy in predicting salaries based on performance.

### 4. "The Scout's Report" (Results)
The model calculated the difference between **Actual Salary** and **Predicted Salary**.
- **Overpaid:** Players earning way more than their stats justify.
- **Undervalued (The Gems):** Players with high stats but low salaries.
- **Output:** A list of the **"Top 5 Undervalued Players"** that clubs should sign immediately.

## 🚀 How to Run

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/your-username/football-valuation.git](https://github.com/your-username/football-valuation.git)
