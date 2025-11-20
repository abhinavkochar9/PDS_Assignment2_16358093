# 📚 Assignment 2: Data Analysis and Statistical Sampling

This repository contains the solution for Assignment 2, which involves two distinct data analysis tasks: data wrangling and feature engineering on a used car dataset (Q1), and statistical analysis, sampling, and bootstrapping on a diabetes dataset (Q2).

---

## 💻 Q1: Used Car Price Analysis

**Data Link:** `https://app.box.com/s/jm6pw202asu4xd3uypwtry2rqk691y1i`

The dataset contains various details and attributes associated with used cars. The **target variable** is the price of the used cars, measured in lakhs.

### Features

* Make and model of the car
* Location or city of sale
* Year of manufacture
* Mileage
* Odometer (kilometers driven)
* Fuel type (petrol or diesel)
* Transmission type (manual or automatic)
* Number of owners
* Engine displacement
* Engine horsepower
* Number of seats
* Price when the car was new

### Tasks

a) **Missing Values:** Look for the missing values in all columns and either impute them (replace with mean, median, or mode) or drop them. **Justify your action** for this task. (4 points)
b) **Unit Removal:** Remove the units from some of the attributes and only keep the numerical values (for example remove `kmpl` from “Mileage”, `CC` from “Engine”, `bhp` from “Power”, and `lakh` from “New\_price”). (4 points)
c) **Categorical Encoding:** Change the categorical variables (“Fuel\_Type” and “Transmission”) into numerical **one-hot encoded values**. (4 points)
d) **Feature Engineering (Mutate):** Create one more feature and add this column to the dataset (e.g., calculate the current age of the car by subtracting “Year” value from the current year). (4 points)
e) **Data Manipulation Operations:** Perform `select`, `filter`, `rename`, `mutate`, `arrange` and `summarize` with `group by` operations (or their equivalent operations in Python) on this dataset. (4 points)

---

## 📊 Q2: Diabetes Dataset Statistical Analysis

**Data Link:** `https://app.box.com/s/7qv44umhw0vnzgmoe9krfkfkv5kf2atv`

The file `diabetes.csv` contains data of 768 patients. We consider this data as the **population** for this assignment.

### Variables

* **Attributes:** Pregnancies, Glucose, BloodPressure, SkinThickness, Insulin, BMI, DiabetesPedigreeFunction, and Age.
* **Response Variable (Outcome):** Binary value (1 indicating diabetes, 0 meaning no diabetes).

### Tasks

a) **Sampling and Comparison (Glucose):** Set a seed (for reproducibility) and take a **random sample of 25 observations**. Find the **mean Glucose** and **highest Glucose** values of this sample and compare these statistics with the population statistics of the same variable. You should use **charts** for this comparison. (5 points)
b) **Percentile Comparison (BMI):** Find the **98th percentile of BMI** of your sample and the population and compare the results using **charts**. (5 points)
c) **Bootstrapping (BloodPressure):** Using **bootstrap (replace=True)**, create **500 samples (of 150 observations each)** from the population and find the **average mean, standard deviation, and percentile** for BloodPressure. Compare this with these statistics from the population for the same variable. Again, you should create **charts** for this comparison. **Report on your findings.** (10 points)

---

## ✅ Submission Details

* Create a **public GitHub repo** and upload the folders for the assignment on the GitHub.
* Submit the link to Canvas.
* The work needs to be organized as **folders and subfolders**.
* Only **notebooks** are acceptable source files (e.g., Jupyter Notebooks or R Markdown/Notebooks).