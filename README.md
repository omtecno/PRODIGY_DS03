🏦 PRODIGY_DS_03 – Bank Marketing Decision Tree
🎯 Overview

Machine Learning project to predict whether a customer will subscribe to a Bank Term Deposit using a Decision Tree Classifier.
Includes EDA, Data Preprocessing, Model Training, and Evaluation on the UCI Bank Marketing Dataset.

📊 Dataset

Source: UCI Bank Marketing Dataset

Records: 45,211 clients

Features: 16 inputs + 1 target

Target: y (Yes/No Deposit)

Class Imbalance: 11.7% Yes, 88.3% No

Key Features: age, job, education, duration, campaign, pdays, poutcome

🛠️ Tech Stack

Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, Jupyter Notebook

⚙️ Methodology

Data Cleaning & EDA

Label Encoding (categorical features)

Outlier Removal (IQR – duration)

Train/Test Split (75/25)

Decision Tree Classifier (Gini)

📈 Results
Metric	Score
Accuracy	89.2%
ROC-AUC	0.91
Precision (Yes)	0.58
Recall (Yes)	0.52
🔑 Top Influential Features

pdays – Recency of last contact

duration – Call length

age – 30–50 most responsive

poutcome – Previous success

campaign – Optimal 1–3 contacts

▶️ How to Run
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
git clone https://github.com/YOUR_USERNAME/PRODIGY_DS_03.git
cd PRODIGY_DS_03
jupyter notebook


Open Bank_Marketing_Decision_Tree.ipynb and run all cells.
