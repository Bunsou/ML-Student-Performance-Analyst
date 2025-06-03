## Hyperparameters

#### Current Hyperparameter Settings

In this initial implementation, most models were run with their default hyperparameter settings, except for a few basic configurations to ensure reproducibility:

- Linear Regression: This model typically does not have hyperparameters that require tuning in its standard form.
- Decision Tree Regressor: random_state=42 was set to ensure that the results are reproducible across different runs.
- Random Forest Regressor: n_estimators=100 (meaning 100 decision trees are built) and random_state=42 were used for consistency.
- Support Vector Regression (SVR): The kernel='rbf' (Radial Basis Function) was used as the default kernel, with other parameters remaining at their default values.

#### Limitations and Future Improvements

This approach represents a baseline implementation, intentionally foregoing advanced hyperparameter optimization for simplicity. For future research and to further enhance model performance and robustness, the following improvements are recommended:

- Grid Search Cross-Validation: Systematically searching through a predefined grid of hyperparameter values for each model to find the optimal combination.
- Cross-Validation (e.g., K-Fold): Employing more robust validation techniques like k-fold cross-validation to get a more reliable estimate of model performance and reduce reliance on a single train-test split.
- Feature Selection: Analyzing feature importance to identify the most predictive variables, which can lead to simpler models, faster training, and potentially improved accuracy by removing noise.
- Advanced Ensemble Methods: Exploring more sophisticated ensemble algorithms such as XGBoost (eXtreme Gradient Boosting) or LightGBM, which often provide state-of-the-art performance in various regression tasks.
  This systematic approach provides a solid, reproducible foundation for predicting student performance based on subject characteristics, with clear pathways for future enhancements.
