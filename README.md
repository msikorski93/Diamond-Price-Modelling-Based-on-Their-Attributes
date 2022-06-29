# Diamond-Price-Modelling-Based-on-Their-Attributes
The purpose of this notebook was to develop an automated function to predict the price of a diamond based on its given features (cut, color, dimensions, etc.). We created a machine learning model which can estimate these values. We needed to find continuous data, so we performed a regression task with supervised learning to find the prices. The task was completed with CRISP-DM approach.

To finalize the regression problem, we implemented the following models and achieved these scores:
* polynomial regressor,
* k-nearest neighbors regressor,
* random forest ensemble,
* AdaBoost (adaptive boosting) ensemble.

| Regressor     | RMSE     | Accuracy | MAE      |
|---------------|----------|----------|----------|
| Polynomial    | 978.5624 | 77.6618  | 592.9765 |
| kNN           | 646.1506 | 84.0253  | 318.3850 |
| Random Forest | 547.1772 | 85.7200  | 278.1653 |
| AdaBoost      | 551.6524 | 84.2118  | 288.2251 |

For the final regressor, we chosen the **random forest ensemble** and deployed it successfully into a serialized file. The estimating function works well and returns predicted values.
