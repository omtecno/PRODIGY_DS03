Bank Deposit Prediction using Decision Tree
📌 Project Overview

This project is a Machine Learning classification model built to predict whether a customer will subscribe to a bank term deposit (yes or no).
The model is trained using the Bank Marketing Dataset and implements Exploratory Data Analysis (EDA) and Decision Tree Classifiers.

📂 Dataset

File Used: bank-additional.csv

Records: 4119

Features: 21 Columns

Target Variable: deposit

The dataset contains customer information such as:

Age

Job

Marital Status

Education

Loan/Housing

Contact Type

Campaign Details

Economic Indicators

Deposit (Target)

🛠 Technologies & Libraries

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

Jupyter Notebook

📊 Exploratory Data Analysis (EDA)

The following visualizations were used:

Histograms – Distribution of numerical features

Bar Plots / Count Plots – Categorical feature frequency

Box Plots – Outlier detection

Correlation Heatmap – Feature relationships

Decision Tree Visualization – Model interpretation

🧹 Data Preprocessing

Steps performed:

Renamed target column y → deposit

Checked for:

Missing Values → None found

Duplicate Rows → None found

Outlier Detection using IQR

Dropped Highly Correlated Columns:

emp.var.rate

euribor3m

nr.employed

Encoded categorical variables using LabelEncoder

Split dataset into:

75% Training

25% Testing

🤖 Machine Learning Models
1. Decision Tree – Gini

Criterion: gini

Max Depth: 5

Min Samples Split: 10

Accuracy: ~89.9%

2. Decision Tree – Entropy

Criterion: entropy

Max Depth: 4

Min Samples Split: 15

Accuracy: ~90.48%

This model performed slightly better than Gini.

📈 Model Evaluation Metrics

Accuracy Score

Confusion Matrix

Precision

Recall

F1-Score

Observation:
Model predicts "No Deposit" very well but struggles slightly with "Yes Deposit" due to class imbalance.

📁 Output Files

clean_data.csv – Cleaned dataset generated after preprocessing.

▶️ How to Run

Install dependencies:

pip install pandas numpy matplotlib seaborn scikit-learn


Open Jupyter Notebook

Run the notebook cells step-by-step

Ensure bank-additional.csv is in the same directory

📌 Future Improvements

Handle class imbalance using SMOTE

Try advanced models:

Random Forest

XGBoost

Logistic Regression

Hyperparameter tuning

Feature scaling

🧠 Conclusion

The Decision Tree model with Entropy provided the best performance.
EDA and feature engineering significantly improved prediction accuracy.

👤 Author

Your Name Here

You can rename the title or author section as needed before uploading to GitHub.

add tables 

Here is an improved README.md with Tables that you can paste directly into GitHub.

Bank Deposit Prediction using Decision Tree
📌 Project Overview

This project builds a Machine Learning Classification Model to predict whether a customer will subscribe to a Bank Term Deposit (Yes / No).
The workflow includes Exploratory Data Analysis (EDA), Data Preprocessing, and Decision Tree Models.

📂 Dataset Information
Attribute	Details
Dataset Name	Bank Marketing Dataset
File Used	bank-additional.csv
Total Rows	4119
Total Columns	21
Target Variable	deposit
Missing Values	0
Duplicate Rows	0
🧾 Feature Types
Data Type	Count	Example Columns
Object (Categorical)	11	job, marital, education
Integer	5	age, duration, campaign
Float	5	euribor3m, nr.employed
🛠 Technologies & Libraries
Tool / Library	Purpose
Python	Programming Language
Pandas	Data Handling
NumPy	Numerical Operations
Matplotlib	Plotting
Seaborn	Visualization
Scikit-learn	Machine Learning
Jupyter Notebook	Development Environment
📊 Exploratory Data Analysis (EDA)
Visualization	Purpose
Histogram	Distribution of numeric data
Bar Plot / Count Plot	Category frequency
Box Plot	Outlier detection
Correlation Heatmap	Feature relationship
Decision Tree Plot	Model interpretation
🧹 Data Preprocessing Steps
Step	Description
Column Rename	y → deposit
Missing Check	No missing values
Duplicate Check	No duplicates
Outlier Removal	IQR Method
Correlation Removal	Dropped highly correlated columns
Encoding	LabelEncoder used
Train/Test Split	75% / 25%
🔗 Highly Correlated Columns Removed
Column Name
emp.var.rate
euribor3m
nr.employed
🤖 Machine Learning Models
Decision Tree – Gini
Parameter	Value
Criterion	Gini
Max Depth	5
Min Samples Split	10
Accuracy	89.9%
Decision Tree – Entropy
Parameter	Value
Criterion	Entropy
Max Depth	4
Min Samples Split	15
Accuracy	90.48%
📈 Model Evaluation Metrics
Metric	Description
Accuracy	Overall correct predictions
Precision	Correct positive predictions
Recall	Ability to detect positives
F1-Score	Balance of precision & recall
Confusion Matrix	True vs Predicted comparison
⚠ Observation – Class Imbalance
Class	Count
No Deposit (0)	3668
Yes Deposit (1)	451

Model predicts “No” better than “Yes” due to imbalance.

📁 Output Files
File Name	Description
clean_data.csv	Preprocessed dataset
▶️ How to Run
Step	Command / Action
Install Libraries	pip install pandas numpy matplotlib seaborn scikit-learn
Open Notebook	Jupyter Notebook
Place Dataset	Same project folder
Run Cells	Sequentially
🚀 Future Improvements
Improvement	Benefit
SMOTE	Handle imbalance
Random Forest	Higher accuracy
XGBoost	Better performance
Hyperparameter Tuning	Optimize model
Feature Scaling	Improve stability
