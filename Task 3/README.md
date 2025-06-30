# 🫀 Heart Disease Prediction using Machine Learning

## 📌 Task Objective
To build a machine learning model that can accurately predict whether an individual is at risk of heart disease based on clinical and demographic health data.

---

## 📊 Dataset Used
- **Name**: Heart Disease UCI Dataset  
- **Source**: [Kaggle - Heart Disease UCI]. 
- **Size**: 1025 samples × 14 features  
- **Target Variable**: `target` (1 = presence of heart disease, 0 = absence)

**Features Include**:
- Age, Sex, Chest Pain Type, Cholesterol, Blood Pressure
- Fasting Blood Sugar, ECG Results, Max Heart Rate, ST Depression
- Exercise-Induced Angina, Slope, Number of Vessels, Thalassemia

---

## 🧠 Models Applied
Two classification models were trained and evaluated:
- **Logistic Regression**
- **Decision Tree Classifier**

**Preprocessing Included**:
- Label Encoding for categorical features
- Feature scaling using `StandardScaler`
- Train-Test Split (80% training, 20% testing)

---

## 📈 Key Results and Findings

### ✔️ Model Evaluation:
| Metric | Logistic Regression | Decision Tree |
|--------|---------------------|----------------|
| **Accuracy** | ~85% | ~79% |
| **ROC-AUC** | ~0.91 | ~0.84 |
| **Confusion Matrix** | Shows good true positive rate | Slight overfitting observed |

### 📊 Feature Importance:
- **Most Influential Features**:
  - Chest Pain Type
  - Maximum Heart Rate
  - ST Depression (`oldpeak`)
  - Thalassemia
  - Exercise-Induced Angina

- Logistic Regression revealed the direction (positive/negative impact), while Decision Tree showed the relative importance.

---

## 🧪 Skills Demonstrated
- Binary classification with real-world medical data
- Exploratory Data Analysis (EDA)
- Model evaluation using ROC, AUC, and confusion matrix
- Interpretation of feature importance to explain predictions
