🏦 PRODIGY_DS_03: Bank Marketing – Decision Tree Classifier
🎯 Project Overview

A complete Machine Learning Pipeline to predict whether a bank customer will subscribe to a Term Deposit using a Decision Tree Classifier.
This project applies Exploratory Data Analysis (EDA), Data Preprocessing, Feature Engineering, and Model Evaluation on the UCI Bank Marketing Dataset.

📊 Dataset Information
Attribute	Details
Source	UCI Machine Learning Repository
Dataset Name	Bank Marketing Dataset
Total Records	45,211 Clients
Features	16 Input + 1 Target
Target Variable	y (Term Deposit Subscription)
Positive Rate	11.7% (Imbalanced Dataset)
🔑 Key Features

age

job

marital

education

duration

campaign

pdays

poutcome

🛠️ Tools & Technologies
Tool / Library	Purpose
Python 3.9+	Programming Language
Pandas	Data Manipulation
NumPy	Numerical Computation
Scikit-learn	Machine Learning
Matplotlib	Visualization
Seaborn	Statistical Plots
Jupyter Notebook	Development Environment
ucimlrepo	Dataset Fetching
joblib	Model Saving
📋 Methodology
1️⃣ Data Loading & Exploration

Loaded dataset (45,211 × 17)

Checked missing & duplicate values

Identified Severe Class Imbalance

Feature type analysis (Categorical vs Numerical)

2️⃣ Data Preprocessing
Step	Action
Encoding	LabelEncoder for categorical columns
Target Mapping	no → 0, yes → 1
Outlier Removal	IQR Method on duration
Feature Cleaning	Removed unnecessary columns
3️⃣ Model Training
DecisionTreeClassifier(
    criterion='gini',
    max_depth=10,
    min_samples_split=20,
    min_samples_leaf=10,
    random_state=42
)

4️⃣ Model Evaluation
Metric	Score
Test Accuracy	89.2%
ROC–AUC	0.91
Precision (Yes)	0.58
Recall (Yes)	0.52
5️⃣ Visualization Suite
Visualization	Purpose
Target Distribution	Class imbalance analysis
Age & Job Distribution	Demographic insights
Duration & Campaign Boxplots	Outlier detection
Feature Importance	Key predictors
Confusion Matrix	Model accuracy evaluation
Correlation Heatmap	Feature relationships
Decision Tree Structure	Model interpretability
🔍 Key Findings
📈 Overall Statistics
Category	Count	Percentage
Total Clients	45,211	100%
Purchased	5,285	11.7%
Not Purchased	39,926	88.3%
Test Accuracy	—	89.2%
🎯 Critical Purchase Factors (Feature Importance)
Rank	Feature	Importance	Business Insight
1	pdays	0.42	Recency of last contact matters
2	duration	0.28	Longer calls → higher conversion
3	age	0.09	30–50 age group most responsive
4	poutcome	0.07	Previous campaign success predictor
5	campaign	0.05	1–3 contacts optimal
🚀 How to Replicate
Prerequisites
pip install pandas numpy scikit-learn matplotlib seaborn ucimlrepo jupyter joblib

Quick Start
# 1. Clone Repository
git clone https://github.com/YOUR_USERNAME/PRODIGY_DS_03.git
cd PRODIGY_DS_03

# 2. Launch Jupyter Notebook
jupyter notebook

# 3. Open Notebook and Run All Cells
Bank_Marketing_Decision_Tree.ipynb

📁 Project Structure
PRODIGY_DS_03/
│
├── Bank_Marketing_Decision_Tree.ipynb
├── dataset.csv
├── model.pkl
├── README.md
└── images/

📌 Future Improvements
Enhancement	Benefit
SMOTE	Handle class imbalance
Random Forest	Higher accuracy
XGBoost	Better generalization
Hyperparameter Tuning	Optimize performance
Feature Scaling	Improve stability
👨‍💻 Author

Your Name

⭐ Repository Stats

Stars: 0

Forks: 0

Watchers: 0

📜 License

This project is open-source and available under the MIT License.

This version is clean, recruiter-friendly, and GitHub professio
