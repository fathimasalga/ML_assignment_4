# ML_assignment_4  REGRESSION & EVALUATION

## Objective:
To evaluates various regression algorithms on the California Housing dataset
to predict median house prices and compare their performance using standard evaluation metrics.
The goal is to implement, evaluate, and compare multiple regression models and identify the best-performing algorithm.

## Dataset: 
- **Source:** sklearn.datasets.fetch_california_housing
- **Target Variable:** Median House Value
- **Features:** 8 numerical housing-related attributes

## Regression Models Implemented
- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor
- Support Vector Regressor (SVR)

## Preprocessing Steps
- Converted dataset to Pandas DataFrame
- Handled missing values
- Feature scaling using StandardScaler
- Encoding using One Hot encoder
- Exploratory Data Analysis (EDA) using histograms and correlation heatmap

## Evaluation Metrics
Each model is evaluated using:
- Mean Squared Error (MSE)
- Mean Absolute Error (MAE)
- R-squared Score (R²)

## Cross-Validation & Hyperparameter Tuning
- 5-fold cross-validation applied to all models
- RandomizedSearchCV used for tuning Random Forest hyperparameters
- Tuned parameters include:
  - n_estimators
  - max_depth
  - min_samples_split
  - min_samples_leaf

## Best Model Selection
Random Forest Regressor performed the best due to:
- Ability to model non-linear relationships
- Lower overfitting compared to Decision Tree
- Higher R² score after hyperparameter tuning
