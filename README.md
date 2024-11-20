# Machine Learning Regression Algorithms

This repository provides an implementation of various machine learning regression algorithms. The purpose of this project is to demonstrate how to work with different regression models, comparing their performance and understanding their functionality.

## Algorithms Included

The following regression models are implemented:

### 1. Random Forest Regressor
- **Description**: Random Forest is an ensemble learning method that combines multiple decision trees to improve prediction accuracy. It works well for both regression and classification tasks.
- **Parameters**:
  - `n_estimators=10`
  - `random_state=42`

### 2. Linear Regression
- **Description**: Linear Regression is one of the simplest models, used for predicting a continuous target variable based on one or more input features. It works well for linear relationships.
- **Parameters**: None

### 3. Decision Tree Regressor
- **Description**: Decision Trees are used for both classification and regression tasks. This model splits the data based on feature values to make predictions. It's intuitive but can suffer from overfitting.
- **Parameters**:
  - `max_depth=10`

### 4. Gradient Boosting Regressor
- **Description**: Gradient Boosting builds an ensemble of decision trees sequentially, with each new tree correcting errors made by the previous one. It's effective but computationally expensive.
- **Parameters**: None

### 5. XGBoost Regressor
- **Description**: XGBoost is an optimized implementation of gradient boosting that is efficient and widely used in machine learning competitions. It performs well on structured/tabular data.
- **Parameters**:
  - `force_row_wise=True`

### 6. LightGBM Regressor
- **Description**: LightGBM is a gradient boosting framework that is faster than XGBoost and scales well for large datasets. It's efficient and performs well in many machine learning tasks.
- **Parameters**: None

### 7. Support Vector Regressor (SVR)
- **Description**: SVR is used to find a hyperplane in an N-dimensional space that best fits the data. It's particularly useful for small datasets or when non-linear models are required.
- **Parameters**: None

## Dependencies

To run this project, you need to install the following Python libraries:

- `scikit-learn`: For Random Forest, Linear Regression, Decision Tree, and SVR.
- `xgboost`: For XGBoost.
- `lightgbm`: For LightGBM.

To install the dependencies, run the following command:

```bash
pip install scikit-learn xgboost lightgbm

