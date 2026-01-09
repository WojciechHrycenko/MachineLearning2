================================================================================
PROJECT: Used Car Price Prediction (Regression) & Rain Prediction (Classification)
COURSE:  Machine Learning 2 (Winter 2025/2026)
================================================================================

1. TEAM MEMBERS
   - Aleksandra Dobosz - 472931
   - Wojciech Hrycenko - 473173

2. OVERVIEW
   Regression part of this project predicts used car prices using a Voting Regressor Ensemble 
   (Random Forest + XGBoost + MLP). The pipeline covers data cleaning, 
   feature engineering, hyperparameter tuning, and error analysis.

   * Target: price (USD)
   * Best R2 Score: ~0.826
   * MAE: ~$3,660

3. SUBMISSION FILES
   - regression_used_cars.ipynb : Regression notebook with code and analysis.
   - regression_used_cars_output.pdf    : PDF export of the notebook output.
   - presentation_slides.pdf  : Presentation slides.
   - vehicles.csv             : Dataset file. - originally from https://www.kaggle.com/datasets/austinreese/craigslist-carstrucks-data - due to the file size limit, it is not included in the repository. Please download it from the original source.

4. INSTALLATION & USAGE (REGRESSION)
   1. Place 'vehicles.csv' in the same folder as the notebook.
   2. Open 'regression_used_cars.ipynb'.
   3. Run all cells sequentially (Cell -> Run All).

================================================================================