# Machine Learning for Solar System Dataset

This repository provides an implementation of various machine learning regression algorithms applied to a solar system dataset. The goal of this project is to demonstrate how different regression models can be used to predict certain features based on the solar system data, such as energy system details, installations, and inverter outputs, among other factors.

## Algorithms Included

The following regression models are implemented and applied to the solar system dataset:

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

## Dataset

The dataset used in this project contains various features of solar energy systems, such as installation details, system size, prices, inverter capacities, and battery ratings. Below is an example of the dataset:

| data_provider_1            | data_provider_2 | system_ID_1 | system_ID_2 | installation_date  | system_size_DC | total_installed_price | rebate_or_grant | customer_segment | expansion_system | ...  |
|----------------------------|-----------------|-------------|-------------|--------------------|----------------|-----------------------|-----------------|-------------------|------------------|------|
| Arkansas State Energy Office | -9999           | -9999       | -9999       | 29-Apr-2010 00:00:00 | 2.016          | 14558.0               | 0.0             | RES               | 0                | ...  |
| Arkansas State Energy Office | -9999           | -9999       | -9999       | 26-Apr-2010 00:00:00 | 3.360          | 26096.0               | 0.0             | RES               | 0                | ...  |
| Arkansas State Energy Office | -9999           | -9999       | -9999       | 20-Apr-2010 00:00:00 | 13.440         | 91139.0               | 0.0             | RES               | 0                | ...  |
| Arkansas State Energy Office | -9999           | -9999       | -9999       | 21-Apr-2010 00:00:00 | 5.520          | 40043.0               | 0.0             | RES               | 0                | ...  |
| Arkansas State Energy Office | -9999           | -9999       | -9999       | 22-Apr-2010 00:00:00 | 2.530          | 21497.0               | 0.0             | RES               | 0                | ...  |

The dataset consists of 78 columns with various features, including but not limited to:

- **System Details**: `system_size_DC`, `total_installed_price`, `rebate_or_grant`
- **Installation Info**: `installation_date`, `customer_segment`
- **Inverter Details**: `built_in_meter_inverter_1`, `output_capacity_inverter_1`
- **Battery Info**: `battery_rated_capacity_kW`, `battery_rated_capacity_kWh`

### Example Data:

| data_provider_1             | installation_date   | system_size_DC | total_installed_price | inverter_loading_ratio | battery_rated_capacity_kW | battery_rated_capacity_kWh |
|-----------------------------|---------------------|----------------|------------------------|------------------------|---------------------------|----------------------------|
| Arkansas State Energy Office | 29-Apr-2010 00:00:00 | 2.016          | 14558.0                | 1.178947               | -9999.0                   | -9999.0                    |
| Arkansas State Energy Office | 26-Apr-2010 00:00:00 | 3.360          | 26096.0                | 1.178947               | -9999.0                   | -9999.0                    |
| Arkansas State Energy Office | 20-Apr-2010 00:00:00 | 13.440         | 91139.0                | 1.178947               | -9999.0                   | -9999.0                    |
| Arkansas State Energy Office | 21-Apr-2010 00:00:00 | 5.520          | 40043.0                | 1.210526               | -9999.0                   | -9999.0                    |
| Arkansas State Energy Office | 22-Apr-2010 00:00:00 | 2.530          | 21497.0                | 1.210526               | -9999.0                   | -9999.0                    |

## Dependencies

To run this project, you need to install the following Python libraries:

- `scikit-learn`: For Random Forest, Linear Regression, Decision Tree, and SVR.
- `xgboost`: For XGBoost.
- `lightgbm`: For LightGBM.

To install the dependencies, run the following command:

```bash
pip install scikit-learn xgboost lightgbm
