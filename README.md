# Flight Price Prediction

## Project Overview
This project uses Machine Learning to predict flight ticket prices based on airline, journey date, source, destination, flight duration, number of stops, and other flight-related features.

The objective is to help customers estimate flight prices and plan their journeys.

## Dataset Information
- Dataset: Flight Fare Dataset
- Original records: 10,683
- Records after cleaning: 10,462
- Original columns: 11
- Features after feature engineering: 18 columns

## Data Preprocessing
- Removed duplicate records.
- Handled missing values.
- Converted flight duration into minutes.
- Extracted journey day and month.
- Extracted departure and arrival hours and minutes.
- Converted total stops into numerical values.
- Applied One-Hot Encoding and StandardScaler.

## Machine Learning Models
Four regression models were trained and evaluated:
1. Linear Regression
2. Decision Tree Regressor
3. Random Forest Regressor
4. Gradient Boosting Regressor

## Model Evaluation

| Metric | Best Result |
|---|---:|
| Best Model | Random Forest |
| MAE | 674.40 |
| RMSE | 1496.91 |
| R² Score | 0.8925 |

Random Forest performed best among the four tested models.

## Feature Importance
The most influential feature was flight duration, with an importance score of approximately 44.17%.

## Project Structure

- `data/` – Original dataset
- `notebooks/` – Python project script
- `outputs/` – Cleaned data, predictions, charts and reports
- `models/` – Saved trained model
- `reports/` – Project summary and challenges report

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib
- VS Code

## Conclusion
The Random Forest Regressor achieved an R² score of approximately 89.25% on the test dataset. It was the best-performing model among the four evaluated models and can be used to estimate flight ticket prices based on the available flight information.

This project demonstrates data cleaning, exploratory data analysis, feature engineering, machine learning model development, evaluation, and model saving.