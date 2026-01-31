🏦 PRODIGY_DS_03 – Bank Marketing
Predicts term deposit subscription using Decision Tree (90.5% accuracy)

📊 Dataset
Records	Features	Target	Balance
4,119	21	deposit	89% No / 11% Yes
Key Features: age, job, duration, pdays, poutcome

🔧 Pipeline
text
EDA → Outlier Removal → Drop High Corr → Label Encoding → Train/Test Split → Decision Tree
📈 Results
Model	Train	Test	Confusion Matrix
DT (gini,d=5)	91.5%	89.9%	-
DT (entropy,d=4)	90.8%	90.5%	[[915,15],[83,17]]
text
[Insert: Histograms | Countplots | Tree Plot | Corr Heatmap]
🚀 Quick Start
bash
# 1. Clone
git clone https://github.com/YOUR_USERNAME/PRODIGY_DS_03.git
cd PRODIGY_DS_03

# 2. Environment
pip install -r requirements.txt

# 3. Run
jupyter notebook bank_analysis.ipynb
