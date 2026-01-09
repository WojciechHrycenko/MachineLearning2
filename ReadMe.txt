================================================================================
PROJECT: Used Car Price Prediction (Regression) & Rain Prediction (Classification)
COURSE:  Machine Learning 2 (Winter 2025/2026)
================================================================================

1. TEAM MEMBERS
   - Aleksandra Dobosz - 472931
   - Wojciech Hrycenko - 473173

2. OVERVIEW
   This submission contains two distinct Machine Learning projects:

   2.1. REGRESSION (Used Car Prices)
   Predicts used car prices using a Voting Regressor Ensemble (Random Forest + 
   XGBoost + MLP). The pipeline covers data cleaning, feature engineering, 
   hyperparameter tuning, and error analysis.
   * Target: price (USD)
   * Best R2 Score: ~0.826
   * MAE: ~$3,660

   2.2. CLASSIFICATION (Rain in Australia)
   Predicts whether it will rain the next day (`RainTomorrow`) based on daily 
   weather observations. The project focuses on handling imbalanced data, 
   managing missing values in time-series data, and maximizing model sensitivity.
   * Target: RainTomorrow (Binary: Yes/No)
   * Best Model: Gradient Boosting
   * Accuracy: [wpisz swój wynik bo nie pamiętam XD]
   * ROC-AUC:  [wpisz swój wynik bo nie pamiętam XD]

3. SUBMISSION FILES
   - regression_used_cars.ipynb          : Regression code and analysis.
   - regression_used_cars_output.pdf     : PDF export of regression output.
   - RainAustraliaClassification.ipynb   : Classification code and analysis.
   - RainAustraliaClassification.pdf     : PDF export of classification output.
   - presentation_slides.pdf             : Presentation slides covering both topics.
   
   DATASETS:
   - vehicles.csv : https://www.kaggle.com/datasets/austinreese/craigslist-carstrucks-data
   - weatherAUS.csv

4. INSTALLATION & USAGE

   4.1. REGRESSION
   1. Place 'vehicles.csv' in the same folder as the notebook.
   2. Open 'regression_used_cars.ipynb'.
   3. Run all cells sequentially.

   4.2. CLASSIFICATION
   1. Open 'RainAustraliaClassification.ipynb'.
   2. Run all cells sequentially.

5. KEY HIGHLIGHTS
   
   REGRESSION:
   - Engineered 'wear_factor' and handled heteroscedasticity via Log-Transformation analysis.
   - Extensive error analysis distinguishing between vintage cars and modern luxury vehicles.
   
   CLASSIFICATION:
   - Advanced preprocessing: Handling location-based missing values and Date parsing.
   - Addressed Class Imbalance (Rain is rare) using appropriate metrics (ROC-AUC, Recall).
   - Comparison of multiple algorithms (Logistic Regression, Random Forest, XGBoost).

================================================================================