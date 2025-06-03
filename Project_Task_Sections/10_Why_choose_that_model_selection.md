## Why This ML Model Choice?

#### Supervised Learning Justification

Supervised learning was chosen for this project because the problem is a regression task. We have "labeled training data," meaning for each set of subject characteristics (input), we know the corresponding student score (output). The objective is to predict these continuous numerical scores, which is the definition of a regression problem.

#### Model Selection Strategy

To identify the most suitable algorithm for this dataset, a comparative approach was adopted. Four different regression algorithms were implemented and evaluated:

- Linear Regression: Selected as an initial baseline model. It's simple, interpretable, and provides a good starting point for understanding basic relationships.
- Decision Tree Regressor: Chosen for its ability to capture non-linear relationships and interactions within the features.
- Random Forest Regressor: An ensemble method that builds multiple decision trees to improve accuracy and reduce the risk of overfitting.
- Support Vector Regression (SVR): Included for its capability to handle complex, non-linear patterns through the use of kernel functions.

This strategy of using multiple algorithms allowed for an empirical comparison, ensuring that the best-performing model for this specific dataset was objectively chosen, rather than relying on assumptions about the data's underlying structure.
