# House Price Analysis & Prediction – King County, USA

## Project Objective
Analyze residential house sales data from King County, USA to identify key factors influencing house prices and build robust regression models for accurate price prediction.

---

## Dataset
Residential housing sales data containing property features such as:
- Location (latitude, longitude, zipcode)
- Living area and lot size
- Bedrooms, bathrooms, floors
- Waterfront, view, and construction quality
- Sale price (target variable)

---

## Tools & Technologies
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  

---

## Project Workflow

### 1. Data Loading & Inspection
- Loaded dataset locally using Pandas
- Reviewed data types, structure, and summary statistics
- Identified missing values and irrelevant identifier columns

### 2. Data Cleaning & Preprocessing
- Removed non-predictive identifier columns
- Handled missing values using mean imputation across numeric features
- Ensured data compatibility for machine learning models

### 3. Exploratory Data Analysis (EDA)
- Analyzed feature distributions and price relationships
- Visualized price impact of waterfront properties
- Examined correlations to identify strong price drivers
- Observed non-linear patterns between features and price

### 4. Feature Selection & Baseline Modeling
- Built baseline linear regression models using:
  - Single features (longitude, sqft_living)
  - Multiple relevant housing features
- Compared model performance using R² score

### 5. Polynomial Regression (Pipeline)
- Implemented a modeling pipeline with:
  - Feature scaling
  - Polynomial feature expansion
  - Linear regression
- Captured non-linear relationships in housing prices

### 6. Model Evaluation
- Split data into training and testing sets
- Applied Ridge regression for regularization
- Evaluated generalization performance on unseen data

### 7. Performance Metrics
- R² Score
- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)

---

## Key Insights
- Living area, location, and construction quality are the strongest drivers of house prices
- Simple linear models underfit real estate data
- Polynomial regression captures non-linear pricing behavior
- Ridge regularization improves model generalization and stability
- The approach supports automated valuation and real-estate pricing systems

---

## Repository Contents
- `house_price_analysis_king_county.ipynb` — Complete analysis and modeling notebook
- `README.md` — Project overview and methodology
- `requirements.txt` — Python dependencies

---

## Future Improvements
- Feature scaling and imputation inside a single pipeline
- Cross-validation for model comparison
- Try tree-based models for non-linear performance gains
