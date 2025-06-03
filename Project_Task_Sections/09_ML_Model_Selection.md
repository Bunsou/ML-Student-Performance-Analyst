## ML Model Selection: Data Collection and Transformation

#### Data Collection Process

Student performance data was sourced from the KIT_DSE_Batch 12_Consolidated_Grade_DataSet.xlsx file. The original dataset was organized in a "wide format," where each row represented a student, and subject scores were spread across multiple columns.

#### Data Transformation Steps

To prepare the raw data for machine learning analysis, the following transformations were performed:

- Step 1: Data Restructuring
  The wide-format data was converted into a "long-format" structure using the pandas.melt() function. This transformed the dataset so that each row represents a unique combination of a student and a subject score, making it more suitable for machine learning analysis.

- Step 2: Feature Engineering
  Based on domain knowledge, new categorical features were manually created to enrich the dataset:

  - Semester: Subjects were classified into "Semester I" (for the first 11 subjects) or "Semester II" (for the remaining subjects).
  - Type of Subject: Subjects were categorized as either "Core Subject" or "Soft Subject" based on curriculum requirements.
  - Nature of Subject: Subjects were classified as either "Theory" or "Practical" based on their teaching methodology.

- Step 3: Data Preprocessing

  - One-Hot Encoding: All categorical variables (e.g., Subject, Semester) were converted into a numerical format (0s and 1s). This process expands each category into a new binary column, which is essential for machine learning models.
  - Standardization (Z-score Normalization): All numerical features were standardized. This scales values to a common range, ensuring that features with larger values don't disproportionately influence the model.

The final processed dataset, ready for model training, had a shape of (814,28) for features (input data) and (814,) for target scores (the output data).

- 814: Represents the total number of individual student-subject records (samples) available.
- 28: Represents the total number of features after the categorical subject, semester, type, and nature features were expanded into numerous binary (0s and 1s) columns through One-Hot Encoding.
