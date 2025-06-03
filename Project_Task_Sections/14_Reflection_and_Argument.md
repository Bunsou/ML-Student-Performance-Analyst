## Reflection and Argument

1. What factors influence KIT students' academic performance?
   The machine learning model uses specific subject characteristics as influencing factors for student academic performance. These factors are:

- Subject: The specific subject being taken (e.g., Mathematics, English).
- Semester: Whether the subject is taken in "Semester I" or "Semester II."
- Type of Subject: If the subject is a "Core Subject" or a "Soft Subject."
- Nature of Subject: If the subject is "Theory" or "Practical" in its methodology.

2. How significant is the difference between theory-based and practical-based subjects in terms of student performance?

The model considers the "Nature of Subject" (Theory or Practical) as a factor when analyzing student performance. This means the model learns to account for any differences in scores associated with these two categories.

However, the visualized data does not directly quantify the "significance" of this difference (e.g., whether students generally score X points higher or lower in practical subjects compared to theory subjects, or if this difference is statistically large). To determine the exact significance, further analysis of the trained model's coefficients or feature importance would be needed, which is not detailed in the provided data.

There are other factors that could be considered significant, such as how the student study, how the lecture is delivered, difficulty of each exam, and the student's background. However, these factors are not included in the current model.

3. What machine learning model can we use to analyze this problem?

Since the goal is to predict continuous numerical student scores, this is a regression problem (a type of supervised learning). The analysis employs a comparative approach using four different regression models:

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- Support Vector Regression (SVR)

By comparing these models, the best-performing one for this specific problem can be identified.

4. What insights can we provide to improve academic outcomes at KIT?

By analyzing the student performance model, we can provide insights to potentially improve academic outcomes at KIT, such as:

- Identifying Performance Patterns: Understanding how student scores vary across different Subjects, Semesters, Types of Subjects (Core/Soft), and Nature of Subjects (Theory/Practical). This could highlight areas where students generally struggle or excel.
- Guiding Curriculum/Teaching Reviews: If the model reveals consistent performance trends related to subject types or nature, it can inform decisions about curriculum adjustments or teaching methodologies to better support student learning.
- Targeted Interventions: Insights from the model could help pinpoint specific subjects or categories of subjects where students might need additional support or different learning approaches to improve their scores.
