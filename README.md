#🧬 Chronic Kidney Disease (CKD) & Diabetic Kidney Disease (DKD) Prediction
Machine Learning + Deep Learning + AutoML Project

This repository contains a complete end-to-end Machine Learning pipeline for CKD (Chronic Kidney Disease) and Stage Prediction, including:

🔍 Data cleaning & preprocessing

📊 EDA & feature engineering

🤖 10+ ML & DL models

⚙ AutoML (AutoGluon)

📈 Evaluation metrics

📡 Full reproducible code in notebooks

🚀 Features

✔ CKD Prediction (binary classification)
✔ CKD Stage Prediction (multi-class)
✔ ML + DL + AutoML comparison
✔ AutoGluon leaderboard
✔ SHAP explainability
✔ Trained models exported
✔ Jupyter Notebook-based experiment

📂 Project Structure
├── data/
│   └── updated_ckd_dataset_with_stages.csv
│
├── notebooks/
│   └── DKD.ipynb
│
├── AutogluonModels/         (ignored using .gitignore)
│
├── results/
│   ├── metrics.csv
│   ├── confusion_matrix.png
│   └── shap_analysis.png
│
├── README.md
└── requirements.txt

🧪 Models Used
🔹 Machine Learning Models
Model	Type	Status
Logistic Regression	ML	✔
Random Forest	ML	✔
Extra Trees	ML	✔
XGBoost	ML	✔
LightGBM	ML	✔
SVM	ML	✔
🔹 Deep Learning Models
Model	Purpose
TabNet	Tabular Deep Learning
TabTransformer	Self-Attention for Tabular Data
🔹 AutoML
Model	Framework
AutoGluon Tabular	AutoML for CKD + Stage Prediction
📊 Model Comparison (Accuracy)

(Example – update with your actual numbers)

Model	Accuracy
Logistic Regression	0.89
Random Forest	0.94
XGBoost	0.95
Extra Trees	0.93
TabNet	0.96
TabTransformer	0.95
AutoGluon (Best Ensemble)	0.97
🛠 Installation
Clone the repository
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>

Install dependencies
pip install -r requirements.txt

▶️ Run the Notebook

Simply open:

notebooks/DKD.ipynb


and run all cells.

📦 Requirements
pandas
numpy
scikit-learn
matplotlib
seaborn
xgboost
lightgbm
autogluon
pytorch
pytorch-tabnet
tab-transformer-pytorch
shap

📘 Dataset Information

The project uses a cleaned CKD dataset with the following features:

Serum Creatinine

GFR

BUN

Serum Calcium

ANA

C3/C4

Hematuria

Oxalate Levels

Urine pH

Blood Pressure

Months

CKD Prediction Label

CKD Stage Label

🧠 Explainability (XAI)

✔ SHAP Feature Importance
✔ SHAP Summary Plot
✔ AutoGluon Feature Importance

📤 Model Export

All trained models are exported automatically:

/AutogluonModels/
/results/models/


(Ignored in Git using .gitignore for large file handling)

📌 Notes

AutoGluon model files are large, so the folder is excluded from git.

You can regenerate all models by simply running the notebook again.

⭐ Contributing

Pull requests are welcome! For major changes, please open an issue first.

🛡 License

MIT License.

🙋‍♂️ Author

mainurrahat178
📧 mainurrahat178@gmail.com
