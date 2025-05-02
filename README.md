# Medical-Cost-Estimator-Using-Regression-
# Insurance Charges Prediction using Linear, Ridge, and Lasso Regression

This project aims to predict medical insurance charges based on demographic and personal health data using three regression models: **Linear Regression**, **Ridge Regression**, and **Lasso Regression**.

## 📊 Dataset

**Source**: [Kaggle - Insurance Dataset](https://www.kaggle.com/datasets/mirichoi0218/insurance)

The dataset contains 1338 records with the following columns:

* `age`: Age of primary beneficiary
* `sex`: Insurance contractor gender
* `bmi`: Body mass index
* `children`: Number of children covered by health insurance
* `smoker`: Smoking status
* `region`: Residential area in the US
* `charges`: Individual medical costs billed by health insurance

---

## 🛠️ Objective

Predict the `charges` using other variables in the dataset by implementing and comparing the performance of:

* Linear Regression
* Ridge Regression
* Lasso Regression

---

## 🧪 Methodology

1. **Data Preprocessing**:

   * Encoded categorical features (`sex`, `smoker`, `region`)
   * Separated features and target (`charges`)
   * Used `train_test_split` (80% train, 20% test)

2. **Model Training**:

   * Fitted the three models on training data
   * Evaluated using Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R² Score

3. **Libraries Used**:

   ```python
   sklearn.linear_model
   sklearn.metrics
   sklearn.model_selection
   numpy
   ```

---

## 📈 Results

| Model             | MSE        | RMSE    | R² Score |
| ----------------- | ---------- | ------- | -------- |
| Linear Regression | 3547820.68 | 5956.34 | 0.8069   |
| Ridge Regression  | 3553618.05 | 5963.75 | 0.8064   |
| Lasso Regression  | 3547939.88 | 5956.53 | 0.8069   |

---

## ✅ Conclusion

* All three models performed similarly.
* **Linear Regression** and **Lasso Regression** had marginally better RMSE and R² than **Ridge**.
* **Lasso** can be preferred for feature selection due to its regularization properties.

---

## 🚀 Future Improvements

* Perform feature scaling
* Explore polynomial regression
* Try ensemble methods (Random Forest, Gradient Boosting)
* Tune hyperparameters using GridSearchCV


