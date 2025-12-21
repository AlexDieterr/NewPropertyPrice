# Property Price Predictor

This project builds a machine learning model to predict the median house value of California districts using census data from 1990. Each data point represents a geographic district rather than an individual home, with features describing income levels, population, housing characteristics, and location.

The goal of the project is to understand what factors influence housing prices and to compare different machine learning models to determine which performs best on this type of tabular data.

---

## Dataset

The dataset comes from the 1990 California census and includes summary statistics for housing districts across the state. Key features include:

- longitude and latitude  
- housing_median_age  
- total_rooms and total_bedrooms  
- population and households  
- median_income (measured in tens of thousands of dollars)  
- ocean_proximity  

The target variable is **median_house_value**, which represents the median home value for each district.

---

## Project Workflow

The project follows a standard machine learning workflow:

1. Data loading and cleaning  
2. Exploratory data analysis (EDA)  
3. Feature engineering, including household-level ratios  
4. Model training and comparison  
5. Hyperparameter tuning  
6. Model evaluation and interpretation  
7. Example predictions on realistic neighborhood scenarios  

---

## Models Used

Several models were trained and evaluated:

- Linear Regression  
- Decision Tree Regressor  
- Random Forest Regressor  
- Tuned Random Forest using RandomizedSearchCV  

Model performance was compared using R² and error metrics.

---

## Results

- The tuned Random Forest model performed best with an R² score of approximately **0.81** on the test set.  
- Median income was the most important feature in predicting housing prices.  
- Location-based features and engineered ratios such as rooms per household also contributed significantly.  
- Residual analysis showed larger errors for higher-priced districts, which is expected given greater variability in expensive housing areas.  

The final model produces reasonable and interpretable predictions that align with real-world expectations.

---

## Technologies Used

- Python  
- pandas, NumPy  
- scikit-learn  
- matplotlib  
- Jupyter Notebook  


---

## Future Improvements

- Try gradient boosting models such as XGBoost or LightGBM  
- Perform more extensive hyperparameter tuning  
- Engineer additional location-based features  
- Explore transformations of the target variable  
- Deploy the model as an interactive web application  

---

## Author

Alex Dieter  
