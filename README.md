# 🎓 Student Performance Predictor

This project aims to predict a student's final grade based on various academic and behavioral features using machine learning models. It demonstrates a complete pipeline—from data preprocessing and feature selection to model training, tuning, and evaluation.

---

## 📂 Dataset

The dataset contains 10 student records with the following features:

- `AttendanceRate`
- `StudyHoursPerWeek`
- `PreviousGrade`
- `ParentalEducation`
- `InternetAccess`
- `SchoolSupport`
- `ExtraCurricularActivities`
- **Target:** `FinalGrade` (numeric)

---

## 🧠 Objective

To build and evaluate regression models that can predict a student's final grade, helping educators identify students at risk and take preventive action.

---

## 🛠️ Tools & Libraries

- Python
- Pandas, NumPy
- Scikit-learn
- Seaborn, Matplotlib

---

## 🔍 Workflow Summary

### 1. Data Preprocessing
- Dropped irrelevant features like `Name`, `Gender`, `StudentID`.
- Handled categorical encoding using `OneHotEncoder`.
- Scaled features using `StandardScaler`.

### 2. Feature Selection
- Correlation matrix analysis.
- Tree-based feature importance evaluation.

### 3. Model Building
Trained three models:
- **Linear Regression**
- **Random Forest Regressor**
- **Support Vector Regressor (SVR)**

### 4. Model Evaluation & Tuning
- Cross-validation (2-fold) to assess stability.
- Hyperparameter tuning using `GridSearchCV`.
- Compared models using:
  - RMSE (Root Mean Squared Error)
  - R² Score

---

## ✅ Final Results

| Model                    | RMSE     | R² Score |
|--------------------------|----------|----------|
| Random Forest Regressor  | 0.2404   | 0.9057   |
| Support Vector Regressor | 0.1796   | 0.9473   |
| Linear Regression        | 0.2601   | 0.8902   |

> **Best Model:** `Support Vector Regressor` with R² Score of **0.9473**

---

## ⚠️ Limitations

- **Small dataset (only 10 samples)**: May cause overfitting or unreliable model generalization.
- Feature coverage is limited; real-world student performance is influenced by many more factors.

---

## 🚀 Future Improvements

- Use a **larger, real-world dataset** (e.g., UCI, Kaggle, or institutional data).
- Add more **relevant features** like psychological metrics, test scores, social environment, etc.
- Implement **deep learning** or **ensemble stacking** approaches for complex patterns.
- Build a **web-based interface** for educators to input data and view predictions.

---

## 📁 Project Structure
📦 Student-Performance-Predictor
├── student-performance-predictor.ipynb
├── README.md
├── requirements.txt
└── dataset/ (optional)

