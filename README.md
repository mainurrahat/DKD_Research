# 🩺 Diabetic Kidney Disease (DKD) Detection & Staging using Machine Learning

This repository presents a complete **end-to-end machine learning pipeline** for the **early detection of Diabetic Kidney Disease (DKD)** and **prediction of DKD stages** using clinical and lifestyle data.

The system follows a **two-stage prediction framework**:
1. **Binary DKD Detection (CKD vs No CKD)**
2. **Multi-class DKD Stage Classification (Stage 1–5)**

Multiple models are evaluated and compared, with **explainability using SHAP** to ensure clinical interpretability.

---

## 📌 Project Objectives

- Detect the presence of Diabetic Kidney Disease (DKD)
- Estimate DKD risk probability
- Predict DKD stage (1–5)
- Handle severe class imbalance using SMOTE
- Compare deep learning and ensemble models
- Provide explainable AI outputs using SHAP

---

## 🧠 Proposed Workflow

1. **Dataset Upload & Exploration**
2. **Data Preprocessing**
   - Feature scaling
   - Encoding
   - Handling missing values
3. **Class Imbalance Handling**
   - SMOTE for binary and stage classification
4. **Model Training**
   - MLP (Primary model)
   - XGBoost (Comparison model)
   - Random Forest (Benchmark model)
5. **Model Evaluation**
   - Accuracy
   - Precision, Recall, F1-score
   - Confusion Matrix
   - ROC Curve
   - Training & Validation Loss Curves
6. **Explainability**
   - Global and patient-level interpretation using SHAP

---

## 📂 Project Structure

DKD_Research/

├── DKD_workflow_rewritten.ipynb # Cleaned & final workflow notebook

├── updated_ckd_dataset_with_stages.csv

├── README.md

├── .gitattributes



## 📊 Dataset Description

- **Total Samples:** 4000
- **Features:** 21 clinical + lifestyle features
- **Binary Labels:**
  - CKD
  - No CKD
- **Stage Labels:**
  - Stage 1 to Stage 5

### Feature Examples
- Serum Creatinine
- GFR
- Blood Urea Nitrogen (BUN)
- Blood Pressure
- Physical Activity
- Smoking & Alcohol Habits
- Family History
- Stress Level

---

## 🤖 Models Used

### 🔹 Primary Model
- **Multi-Layer Perceptron (MLP)**
  - Separate models for:
    - Binary DKD detection
    - DKD stage classification
  - Trained for **600 epochs**

### 🔹 Comparison Models
- **XGBoost**
- **Random Forest**

---

## 📈 Model Performance Summary

### ✅ Binary DKD Detection

| Model | Accuracy |
|------|---------|
| MLP | **98.5%** |
| Random Forest | 98.9% |
| XGBoost | **99.0%** |

### ✅ DKD Stage Classification

| Model | Accuracy |
|------|---------|
| MLP | **94.6%** |
| Random Forest | **99.4%** |
| XGBoost | **99.3%** |

---

## 🔍 Explainable AI (SHAP)

- SHAP is used for:
  - Global feature importance
  - Patient-level prediction explanation
- Helps understand:
  - Which features contribute most to DKD detection
  - Why a specific DKD stage is predicted

---

## 🧪 Example Prediction Output

```
{
  "dkd_detected": true,
  "dkd_risk_probability": 1.0,
  "predicted_stage": 1,
  "stage_probabilities": {
    "1": 1.0,
    "2": 2.2e-12,
    "3": 2.3e-30,
    "4": 0.0,
    "5": 0.0
  }
}
```
⚙️ Installation & Usage

1️⃣ Clone Repository
```
git clone https://github.com/mainurrahat/DKD_Research.git
cd DKD_Research
```

2️⃣ Install Dependencies
```
pip install -r requirements.txt
```

3️⃣ Run Notebook

Open and run:

```
DKD_workflow_rewritten.ipynb
```
🧾 Research Contribution

Two-stage DKD prediction pipeline

Robust handling of class imbalance

Deep learning vs ensemble model comparison

Explainable AI integration for healthcare trust

Suitable for academic research and clinical decision support

📌 Future Improvements

External dataset validation

LightGBM comparison

Model calibration analysis

Deployment as a web-based clinical decision support system
