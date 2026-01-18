## Project Overview
This project explores the implementation of **Linear** and **Polynomial Regression** models on two engineering datasets. The objective was to evaluate how increasing model complexity (degrees 1-4) affects predictive performance and generalization.

---

## Part 1: Fuel Consumption & Horsepower
In this section, I modeled the relationship between **Fuel Economy (MPG)** and **Horsepower**.

* **Model Results**: The baseline Linear Regression model performed exceptionally well, achieving a **Test $R^2$ of 0.912**.
* **Complexity Analysis**: Increasing the polynomial degree to 4 only marginally improved the Test $R^2$ to **0.913**. 
* **Conclusion**: Because the relationship is predominantly linear, a simple model is sufficient and preferred to avoid unnecessary computational cost.

---

## Part 2: Electricity Consumption & Weather
This analysis focused on predicting daily electricity demand based on weather features like wind speed and temperature.

* **Non-linear Dynamics**: Linear Regression achieved a low **Test $R^2$ of 0.299**, failing to capture the complex, non-linear energy demands driven by heating and cooling.
* **Extreme Overfitting**: At **Degree 4**, the model completely failed on the test set, with the **Test $R^2$ crashing to -33.31**. 
* **Key Finding**: This highlights a classic case of overfitting where the model "memorized" the training noise instead of learning the actual physical relationship.



---

## Technical Implementation
* **Language**: Python (Google Colab)
* **Libraries**: `scikit-learn`, `pandas`, `numpy`
* **Data Split**: 70% Training / 30% Testing
