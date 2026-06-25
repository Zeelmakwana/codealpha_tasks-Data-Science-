# CODEALPHA Internship Tasks

This repository contains all 4 data science tasks completed during the CODEALPHA  internship. Each task covers a different real-world machine learning or data science problem.

---

## Task 1 - Iris Flower Classification

**Dataset:** Iris.csv (150 rows, 4 features)

The Iris dataset contains measurements of 3 species of iris flowers — Setosa, Versicolor, and Virginica. The goal is to classify the species based on sepal and petal dimensions.

**What was done:**
- Loaded and explored the dataset
- Checked for null values (none found)
- Encoded the target column (Species) using LabelEncoder
- Split data into 80% train and 20% test
- Trained and compared 5 models:
  - Logistic Regression — 97.3% (cross-val)
  - K-Nearest Neighbors — 97.3% (cross-val)
  - Decision Tree — 96.0% (cross-val)
  - Random Forest — 96.0% (cross-val)
  - SVM — 96.7% (cross-val)
- All models achieved 100% accuracy on test set
- Made a sample prediction on new flower data

**Files:** `Iris_classification.ipynb`, `Iris.csv`

---

## Task 2 - Unemployment Analysis in India

**Dataset:** Unemployment in India.csv, Unemployment_Rate_upto_11_2020.csv

This task analyzes unemployment trends in India, especially the impact of the COVID-19 pandemic on employment.

**What was done:**
- Loaded and cleaned both datasets
- Plotted unemployment rate distribution (histogram)
- Identified states with highest and lowest unemployment rates
- Analyzed monthly trend — found a major spike in April 2020 during lockdown
- Compared average unemployment rate before and after COVID:
  - Before COVID: ~9.5%
  - After COVID: ~17.8%
- Analyzed unemployment by region:
  - North India most affected (15.89%)
  - West India least affected (8.24%)
- Found Haryana had the highest and Meghalaya had the lowest unemployment rate

**Key Finding:** COVID-19 nearly doubled the unemployment rate in India, with the worst impact in April 2020.

**Files:** `Unemployment_Analysis.ipynb`, `Unemployment in India.csv`, `Unemployment_Rate_upto_11_2020.csv`, `Analysis.txt`

---

## Task 3 - Car Price Prediction

**Dataset:** car data.csv

This task builds a model to predict used car selling prices based on features like year, fuel type, transmission, and more.

**What was done:**
- Loaded and explored the car dataset
- Cleaned data and handled categorical columns
- Feature engineering and selection
- Trained regression models to predict car selling price
- Evaluated model performance

**Files:** `Car_Price_Prediction.ipynb`, `car data.csv`

---

## Task 4 - Sales Prediction

**Dataset:** Advertising.csv (200 rows)

This task predicts product sales based on advertising budget spent on TV, Radio, and Newspaper.

**What was done:**
- Loaded and explored the dataset (no null values)
- Plotted correlation heatmap — TV has highest correlation (0.78) with Sales
- Plotted scatter plots for each advertising channel vs Sales
- Split data into 80% train and 20% test
- Trained 3 models:
  - Linear Regression — R2: 0.899, RMSE: 1.78
  - Ridge Regression — R2: 0.899, RMSE: 1.78
  - Random Forest — R2: 0.981, RMSE: 0.77
- Random Forest is the best model with highest R2 and lowest error
- Plotted actual vs predicted sales for all 3 models
- Plotted feature importance — TV and TV×Radio interaction most important
- Made a live prediction: TV=200, Radio=40, Newspaper=30 → Predicted Sales printed

**Key Finding:** TV advertising has the strongest impact on sales. Radio also contributes significantly. Newspaper has the weakest effect.

**Files:** `Sales_Prediction.ipynb`, `Advertising.csv`

---

## Tools and Libraries Used

- Python 3
- pandas, numpy
- matplotlib, seaborn
- scikit-learn (sklearn)
- Jupyter Notebook
