# House Price Prediction 🏠

An end-to-end regression project predicting house prices based on area-level 
features, built as the final capstone project for my Data Science internship.

## Dataset
Source: [USA_Housing.csv - Kaggle](https://www.kaggle.com/datasets/aariyan101/usa-housingcsv)
5,000 rows, 6 features (Income, House Age, Rooms, Bedrooms, Population) → Price

## Process
1. **Data Cleaning** — dropped non-numeric Address column, verified no missing 
   values or duplicates
2. **EDA** — univariate/bivariate analysis, correlation heatmap, IQR-based 
   outlier detection
3. **Modeling** — Linear Regression with train/test split
4. **Evaluation** — R², MAE, RMSE, residual analysis, actual-vs-predicted 
   visualization
5. **Feature Scaling** — used StandardScaler to enable fair coefficient 
   comparison across features

## Key Results
- **R² = 0.918** — model explains ~92% of price variance
- **Avg. Area Income** is the strongest predictor of price, confirmed by both 
  correlation analysis and standardized model coefficients
- Model shows well-behaved, zero-centered residuals with no systematic bias

## Key Insight
Initial unscaled coefficients appeared to contradict EDA findings — a valuable 
lesson in why feature scaling matters before interpreting regression coefficients.

## Tools Used
Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, Google Colab

## Author
Mohammed Aslansha S — Data Science Intern @ Codomax Digital Solutions
