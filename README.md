# California Housing Price Prediction with Linear Regression
This project demonstrates how to build and evaluate linear regression models (including Ridge and Lasso variants) to predict housing prices using the California housing dataset from sklearn.datasets.
# Project Overview
The notebook walks through:
- Data loading and preprocessing
- Model training using Linear, Ridge, and Lasso regression
- Evaluation using cross-validation and R² score
- Visualization of prediction errors
  # Dataset
- Source: California Housing dataset via sklearn.datasets.fetch_california_housing
- Features: Median income, house age, average rooms, population, etc.
- Target: Median house value
  # Setup and Dependencies
  pip install numpy pandas matplotlib seaborn scikit-learn


# Model Workflow
1. Load and Prepare Data
- Data fetched from sklearn and converted to a DataFrame
- Features (X) and target (Y) separated
2. Train-Test Split
- 70:30 ratio using train_test_split with a fixed random seed
3. Data Standardization
- StandardScaler applied to normalize the features
4. Model Training
- Linear Regression model trained and validated via cross-validation
- Performance metric: Negative Mean Squared Error (MSE)
5. Evaluation
- Predicted vs actual results plotted using KDE
- r2_score computed for model accuracy
6. Ridge Regression
- Hyperparameter tuning using GridSearchCV
- Best alpha selected from [1, 2, ..., 50]
- Predictions visualized and scored
7. Lasso Regression
- Similar tuning and evaluation as Ridge
- Best alpha selected from [1, 2, ..., 60]
  # Results
- All three models evaluated based on error distribution and R² score
- Ridge and Lasso provide regularization, improving performance by minimizing overfitting
  # Highlights
- Effective comparison of multiple linear models
- Use of cross-validation for robust model scoring
- Visual insights with Seaborn KDE plots
