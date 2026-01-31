Bank Marketing Dataset Analysis
This repository contains a complete Exploratory Data Analysis (EDA) and Decision Tree Classification pipeline for the Bank Marketing dataset. Predicts term deposit subscription (yes/no) using customer data.

📊 Dataset Overview
Attribute	Type	Description	Unique Values
age	Numeric	Customer age	18-88
job	Categorical	Customer occupation	12 categories
marital	Categorical	Marital status	married, single, divorced
deposit	Target	Term deposit (yes/no)	3668 no, 451 yes
duration	Numeric	Call duration (seconds)	0-3643
Dataset Shape: 4,119 rows × 21 columns [No missing values, no duplicates]

📈 Key Findings
Metric	Value
Data Balance	89% No (3668), 11% Yes (451)
Best Model	Decision Tree (90.48% Test Accuracy)
High Correlation	euribor3m ↔ emp.var.rate (0.97)
Outliers Removed	age, campaign, duration
text
[Graph Space: Insert df.hist() - Numeric Distributions (magenta bars)]
🔧 Preprocessing Steps
Delimiter Fix: pd.read_csv("bank-additional.csv", delimiter=';')

Column Rename: y → deposit

Outlier Removal: IQR method on age, campaign, duration

Multicollinearity: Dropped emp.var.rate, euribor3m, nr.employed

Encoding: LabelEncoder for all categorical variables

Train/Test Split: 75/25 (3089/1030 samples)

text
[Graph Space: Insert sns.countplot() - Categorical Distributions (viridis palette)]
🤖 Model Performance
Model	Train Score	Test Score	Confusion Matrix
dt (gini, depth=5)	91.49%	89.90%	-
dt1 (entropy, depth=4)	90.81%	90.48%	[
​,
​]
text
[Graph Space: Insert plot_tree(dt1) - Decision Tree Visualization (colored nodes)]
[Graph Space: Insert sns.heatmap() - Correlation Matrix (Set3 colormap)]
📁 File Structure
text
bank-marketing-analysis/
│
├── bank-additional.csv      # Original dataset
├── clean_data.csv          # Cleaned/exported data
├── bank_analysis.ipynb     # Complete Jupyter notebook
└── README.md              # This file
🚀 Quick Start
bash
# Clone & Open
git clone <your-repo>
cd bank-marketing-analysis
jupyter notebook bank_analysis.ipynb
📊 Results Summary Table
Stage	Shape	Action
Original	(4119, 21)	Load data
Post-Outliers	(4119, 21)	IQR cleaning
Post-Drop Corr	(4119, 18)	Remove multicollinearity
Encoded	(4119, 18)	Label encoding
Train/Test	3089/1030	75/25 split
text
[Graph Space: Insert df.plot(kind='box') - Before/After Outlier Removal]
