# Data Science & Analytics: Assignment 2 - Used Car Price Prediction and Diabetes Dataset Analysis

## 🎯 Assignment Goal

This repository contains the solution notebooks for **Assignment 2**, which focuses on practical data wrangling, feature engineering, exploratory data analysis (EDA), and statistical sampling/bootstrapping using two distinct datasets. The primary tools used are **Python** (with libraries like Pandas, NumPy, Matplotlib, and Seaborn) or **R** (with libraries like Tidyverse).

The assignment is divided into two main sections:

1.  **Q1: Used Car Price Analysis and Data Preparation** (Focus on data cleaning and feature engineering).
2.  **Q2: Diabetes Dataset Statistical Analysis** (Focus on sampling, comparison with population statistics, and bootstrapping).

## 🗃️ Repository Structure

The assignment is organized into distinct folders for clarity and navigation.

| Folder | Description |
| :--- | :--- |
| `Q1_Used_Cars_Analysis/` | Contains the notebook for Question 1, addressing data cleaning, feature engineering, and data manipulation operations on the used cars dataset. |
| `Q2_Diabetes_Stats/` | Contains the notebook for Question 2, addressing statistical sampling, comparison, and bootstrapping techniques on the diabetes dataset. |
| `data/` | (Optional, but recommended) This is where the raw data files (`used_cars_data.csv` and `diabetes.csv`) are stored for reproducible access within the notebooks. |

## 🚀 Q1: Used Car Price Analysis and Data Preparation

The notebook in `Q1_Used_Cars_Analysis/` performs the required preparation steps on the used cars dataset, where the target variable is the car price in lakhs.

### Key Tasks Completed

1.  **Missing Value Treatment:** Identified and treated missing values across all columns. **(Requirement 1a)**
    * *Justification for the chosen imputation/dropping method is documented within the notebook.*
2.  **Unit Removal:** Cleaned numerical features by removing non-numeric units (e.g., 'kmpl', 'CC', 'bhp', 'lakh') to prepare them for modeling. **(Requirement 1b)**
3.  **Categorical Encoding:** Converted the categorical features **'Fuel\_Type'** and **'Transmission'** into numerical format using **One-Hot Encoding**. **(Requirement 1c)**
4.  **Feature Engineering:** Created a new feature, **`Car_Age`**, by calculating the difference between the current year and the car's **'Year'** of manufacture. **(Requirement 1d)**
5.  **Data Manipulation Operations:** Demonstrated proficiency in: **(Requirement 1e)**
    * `select` / Column selection
    * `filter` / Row filtering
    * `rename` / Column renaming
    * `mutate` / Feature creation
    * `arrange` / Sorting
    * `summarize` with `group_by` / Aggregation by category

## 📊 Q2: Diabetes Dataset Statistical Analysis

The notebook in `Q2_Diabetes_Stats/` focuses on statistical sampling and comparison techniques using the `diabetes.csv` dataset, which contains 8 attributes and a binary 'Outcome' variable.

### Key Tasks Completed

1.  **Random Sampling and Comparison (Glucose):** **(Requirement 2a)**
    * Set a random seed for reproducibility.
    * Drew a random sample of **25 observations**.
    * Calculated the **mean** and **highest** Glucose values for the sample.
    * Compared these sample statistics against the corresponding **population** statistics.
    * *Comparison results are visualized using charts.*
2.  **Percentile Comparison (BMI):** **(Requirement 2b)**
    * Calculated the **98th percentile** of BMI for both the sample and the population.
    * *Comparison results are visualized using charts.*
3.  **Bootstrapping Analysis (BloodPressure):** **(Requirement 2c)**
    * Generated **500 bootstrap samples** (with replacement) of **150 observations** each from the population.
    * Calculated the **average mean, standard deviation, and percentile** of BloodPressure from the bootstrap distribution.
    * Compared these bootstrap statistics against the corresponding **population** statistics for BloodPressure.
    * *Comparison results are visualized using charts, and a detailed finding report is included in the notebook.*

## 💻 Technical Stack

* **Programming Language:** Python (or R)
* **Libraries:**
    * Pandas (Data Manipulation)
    * NumPy (Numerical Operations)
    * Matplotlib / Seaborn (Data Visualization)
    * Scikit-learn (Optional, for encoding)

## 📌 How to Run the Notebooks

1.  **Clone the Repository:**
    ```bash
    git clone [YOUR_GITHUB_REPO_LINK]
    ```
2.  **Download Data:** Ensure the data files (linked in the assignment prompt) are downloaded and placed in the appropriate `data/` folder, or modify the file paths in the notebooks.
3.  **Install Dependencies:** Install the required Python/R libraries (e.g., `pip install pandas numpy matplotlib seaborn` for Python).
4.  **Run:** Open and run the notebooks (`Q1_Used_Cars_Analysis.ipynb` and `Q2_Diabetes_Stats.ipynb`) using Jupyter Notebook or VS Code.

## 🔗 Data Sources

* **Q1 Data (Used Cars):** `https://app.box.com/s/jm6pw202asu4xd3uypwtry2rqk691y1i`
* **Q2 Data (Diabetes):** `https://app.box.com/s/7qv44umhw0vnzgmoe9krfkfkv5kf2atv`