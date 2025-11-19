# Student_Performance_Prediction
This project focuses on analyzing university student performance data to uncover key factors influencing academic outcomes and to build predictive models that estimate student scores and grades based on demographic, behavioral, and academic inputs. The dataset covers diverse student attributes, providing a rich foundation for both descriptive and predictive analytics.

# Objective
- To identify and understand the significant features impacting student academic success.
- To clean, preprocess, and enrich the student dataset for quality analysis.
- To construct and evaluate machine learning models that predict academic performance and provide insights for targeted interventions
# Steps Included
1. Data Loading & Initial Exploration
Imported essential libraries: pandas, numpy, matplotlib, seaborn, scikit-learn, etc.
Loaded the dataset C Performance Dataset.csv and inspected its columns, data types, and sample records.

2. Data Cleaning & Preprocessing
Checked for and removed missing values and handled inconsistent/categorical entries (e.g., standardized parent education levels).
Removed duplicates based on student identifiers and multiple columns to ensure data integrity.
Addressed outliers through visualization and subsequent filtering.
Conducted statistical summaries to understand distribution and central tendencies of all columns.​

3. Feature Engineering
Created new meaningful features such as StudyEfficiency (linking study hours and attendance) and ParentSupportScore (numerical encoding of parent's education level).
Applied one-hot encoding to categorical variables (e.g., extracurricular activities, parental education, family income).

4. Feature Scaling
Standardized numerical features using StandardScaler to ensure model compatibility and fair comparison within algorithms.​

5. Model Building & Evaluation
Split data into training/testing sets.
Modeled student performance using supervised regression algorithms: Linear Regression, Ridge, Lasso, Random Forest, Gradient Boosting.
Used GridSearchCV for hyperparameter tuning of Random Forest to optimize prediction accuracy.
Evaluated models using MAE, MSE, and R2 scores and presented a confusion matrix for grade classification.​

6. Interpretation & Visualization
Analyzed feature importances of the best-performing model (Random Forest), highlighting which attributes most influence final scores and grades.

# Final Insights
Key Findings: Academic performance is most strongly predicted by total scores, project scores, midterm scores, assignment averages, and participation rates. Behavioral traits such as study hours, parental education (as ParentSupportScore), family income, and attendance also significantly impact outcomes.​
Model Performance: The tuned Random Forest achieved a high R2 score (≈ 0.85), indicating strong predictive power. MAE and MSE were low, denoting precise regression.​
Interventions: Insights support targeted academic support for students with lower project, participation, or assignment scores. Family background and behavioral variables highlight groups who may benefit from additional resources.



Visualized results and diagnostics using box plots, heatmaps, and feature importance charts.

