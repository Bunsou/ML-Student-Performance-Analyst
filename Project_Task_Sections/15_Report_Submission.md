## Report Submission: KIT Student Performance Analysis Project

Objective: To develop a machine learning model capable of predicting KIT student academic performance based on subject characteristics.

1. Dataset Overview:
   The project utilized student performance data from the KIT_DSE_Batch 12_Consolidated_Grade_DataSet.xlsx. This data was transformed into a suitable format, engineered with new features (Semester, Subject Type, Subject Nature), and preprocessed using One-Hot Encoding and standardization. The final dataset consisted of 814 student-subject records with 28 features used for modeling.

2. Model Selection:
   Addressing a regression problem (predicting continuous scores), a comparative analysis was performed using Linear Regression, Decision Tree, Random Forest, and Support Vector Regression models. Linear Regression was selected due to its simplicity and interpretability, serving as a clear baseline for understanding factor influence.

3. Methodology:
   The dataset was split into 80% for training and 20% for testing to evaluate generalization. Model performance was assessed using standard metrics: R² Score, Mean Absolute Error (MAE), and Root Mean Square Error (RMSE). Models were trained with default hyperparameters.

Model Performance & Summary:
The Linear Regression model achieved an R² score of 0.5875, indicating that it explains approximately 58.75% of the variance in student performance. This performance level is considered fair-to-good. The accuracy is primarily influenced by the fact that the model relies solely on four high-level subject features. To achieve better prediction accuracy, incorporating more diverse factors (e.g., student-specific attributes like attendance, prior academic history, or instructor details) would be essential.
