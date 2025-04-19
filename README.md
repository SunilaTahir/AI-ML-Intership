This is my first github repository containing 3 tasks of my very first internship at "Developers' Hub". Here's a short summary of these tasks

Task 1: Combined Data Analysis Summary (Preliminary)
Dataset Overview:
•	Two datasets were used:
o	bank.csv: For classification task (Task 2)
o	all_seasons.csv: For regression task (Task 3)
Initial Analysis Steps:
•	Loaded both datasets using Pandas.
•	Checked shapes, data types, and missing values.
•	Generated summary statistics using describe().
•	Visualized data distributions using histograms.

Task 2: Bank Marketing Campaign Success Prediction (Binary Classification)
Objective: Predict whether a customer will subscribe to a term deposit using classification models.
Data Preprocessing:
•	Loaded bank.csv dataset.
•	No missing values were found.
•	Categorical features were encoded using LabelEncoder.
•	All numerical features were scaled using StandardScaler.
Feature Selection:
•	Used SelectKBest with mutual_info_classif to select the 10 most relevant features.
•	Feature importance was visualized using bar charts.
Model Training & Evaluation:
•	Trained and evaluated the following models:
o	Logistic Regression
o	Decision Tree Classifier
o	Random Forest Classifier
•	Used 5-fold cross-validation for reliable model evaluation.
•	Metrics used:
o	Accuracy
o	Precision
o	Recall
o	F1-Score
•	Random Forest showed the best performance overall.
Feature Impact:
•	Random Forest's feature_importances_ were used to identify top predictors of customer subscription.
•	Plotted top features using bar graphs for interpretation.

Task 3: NBA Player Performance Prediction (Regression)
Objective: Predict NBA player performance using regression models.
Data Preprocessing and EDA:
•	Loaded all_seasons.csv dataset.
•	Checked data types and null values.
•	Explored distributions of pts, ast, reb, etc. using histograms.
•	Analyzed feature correlation with a heatmap.
Feature Engineering:
•	Created a new target variable Performance_Index:
•	Performance_Index = pts + ast + reb + stl + blk - tov
•	Selected numeric features for modeling.
•	Standardized features using StandardScaler.
Model Training & Evaluation:
•	Split data into training and testing sets (80/20).
•	Trained the following regression models:
o	Linear Regression
o	Ridge Regression
•	Metrics used:
o	R-squared (R²)
o	Mean Absolute Error (MAE)

