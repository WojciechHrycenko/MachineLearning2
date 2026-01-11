# Machine Learning 2

![Project Status](https://img.shields.io/badge/Status-In%20Progress-yellow)
![Course](https://img.shields.io/badge/Course-Machine%20Learning%202-blue)
![Tools](https://img.shields.io/badge/Tools-Python%20-green)

## Project Overview

This repository contains the coursework and projects developed for the **Machine Learning 2** course. The primary objective was to apply and evaluate various machine learning techniques on real-world datasets, specifically focusing on classification and regression problems.

## Authors
* **Aleksandra Dobosz**
* **Wojciech Hrycenko**

---

## Repository Contents

### 1. Classification: Rain Prediction in Australia
**Directory:** `Classification/`

**Objective**
The goal of this project was to develop a binary classification model to predict whether it will rain the following day in Australia (target variable: `RainTomorrow`), based on daily meteorological observations.

**Dataset**
The project utilizes the `weatherAUS.csv` dataset, which includes features such as temperature, rainfall, sunshine, wind gusts, humidity, and pressure.

**Methodology**
* **Data Analysis & Preprocessing:** Addressed missing values and analyzed variable distributions (noting significant skewness in rainfall data).
* **Modeling:**
    * Decision Tree Classifier
    * Random Forest Classifier
    * Gradient Boosting Classifier
* **Techniques:** Implemented class weighting (`class_weight='balanced'`) to mitigate the imbalance between rainy and non-rainy days.
* **Evaluation:** Performance assessment focused on **Recall** and **F1-score** for the positive class to minimize the risk of failing to predict rainfall. The Gradient Boosting model, following decision threshold optimization, yielded the most robust results.

### 2. Regression: Used Car Price Prediction
**Directory:** `Regression - Used Cars/`

**Objective**
This project aimed to build a regression model to estimate the market price of used vehicles based on data scraped from Craigslist.

**Dataset**
The analysis used the `vehicles.csv` dataset, comprising millions of vehicle listings from the United States.
> **Note:** Due to file size limitations, the dataset is not hosted in this repository. It can be downloaded from Kaggle:
> [**Used Cars Dataset (Craigslist)**](https://www.kaggle.com/datasets/austinreese/craigslist-carstrucks-data)

**Methodology**
* **Data Quality Assessment:** Conducted a thorough analysis of missing data and unique value counts.
* **Preprocessing:**
    * **Dimensionality Reduction:** Removed columns with excessive missingness (e.g., `county`, `size`) and irrelevant identifiers (`VIN`, `url`).
    * **Imputation:** Filled missing categorical data with an 'unknown' placeholder.
    * **Outlier Detection:** Filtered data to realistic ranges for price ($500 - $150k), manufacturing year (1990-2025), and odometer readings.
* **Modeling:**
    * Linear Regression
    * Random Forest Regressor
    * XGBoost Regressor
    * Neural Networks (MLP Regressor)
    * Voting Regressor (Ensemble method)
* **Evaluation:** Models were compared using Mean Absolute Error (MAE), Mean Squared Error (MSE), and the R-squared (R2) coefficient.

---

## Technologies and Libraries

The project was developed in **Python**, utilizing the following key libraries:

* **Pandas & NumPy:** For efficient data manipulation and numerical analysis.
* **Scikit-learn:** For model training, preprocessing pipelines, and evaluation metrics.
* **XGBoost:** For high-performance gradient boosting algorithms.
* **Matplotlib & Seaborn:** For exploratory data analysis and result visualization.
* **Jupyter Notebook:** Used as the interactive development environment.

## Usage Instructions

1.  Clone this repository to your local machine.
2.  Ensure all required dependencies are installed (refer to library list above).
3.  **For Regression Project:** Download the `vehicles.csv` file from the Kaggle link provided above and place it in the `Regression - Used Cars/` directory.
4.  Navigate to the respective directories (`Classification` or `Regression`) and execute the Jupyter Notebooks (`.ipynb`) to view the analysis and reproduce the models.
