# 🎓 Student Performance Analysis & Prediction
> Analyzing student academic performance and predicting pass/fail outcomes using Machine Learning

![Python](https://img.shields.io/badge/Python-3.13-blue) ![Scikit--learn](https://img.shields.io/badge/Scikit--learn-Latest-orange) ![Pandas](https://img.shields.io/badge/Pandas-Latest-green) ![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

---

## 📌 Overview
This project analyzes a real-world student dataset containing **395 student records** to identify key factors affecting academic performance and builds a Machine Learning model to predict whether a student will **pass or fail** their final exam using 13 meaningful features.

---

## 📊 Part 1 — Exploratory Data Analysis

### 📈 Grade Distribution
- Analyzed final grade (G3) distribution across all 395 students
- Average final grade: **10.42 / 20**
- **265 students passed (67%)** and **130 students failed (33%)**

### 📚 Study Time vs Final Grade
- Students with higher study time scored significantly better
- Clear positive trend — **more study time = higher grades**
- Boxplot used to visualize grade spread across study groups

### ❌ Past Failures vs Final Grade
- Students with no past failures scored highest (median ~12)
- Clear negative trend — **more failures = lower final grade**
- Past failures identified as strongest negative factor

### 🗺️ Correlation Heatmap
- Analyzed relationships between all 16 numerical features
- **G1 (0.90) and G2 (0.80)** are strongest predictors of final grade
- Past failures showed strongest negative correlation (-0.36) with G3

---

## 🤖 Part 2 — Machine Learning

### 🔧 Data Preparation
- Selected **13 meaningful features** based on correlation analysis
- Encoded categorical columns (higher, internet, romantic) using Label Encoding
- Split data: **80% training (316 students)** and **20% testing (79 students)**
- Used stratified split to maintain Pass/Fail ratio in both sets

### 🏆 Model Results

| Model | Accuracy | Correct Predictions | Wrong Predictions |
|-------|----------|--------------------|--------------------|
| 🥇 Logistic Regression | **89%** | 70 / 79 | 9 / 79 |
| 🥈 Decision Tree | 86% | 68 / 79 | 11 / 79 |

### 📋 Logistic Regression — Confusion Matrix
```
              Predicted Fail    Predicted Pass
Actual Fail        25                1
Actual Pass         8               45
```

---

## 🔍 Key Findings
✅ **G1 and G2 grades** are the strongest predictors of final performance

✅ Students with **zero past failures** perform significantly better

✅ **Higher study time** consistently leads to better final grades

✅ **Logistic Regression** outperformed Decision Tree with 89% accuracy

✅ Social factors like going out and alcohol consumption negatively impact grades

---

## 🛠️ Tools & Libraries

| Tool | Purpose |
|------|---------|
| 🐍 Python 3.13 | Core programming language |
| 🐼 Pandas | Data cleaning & transformation |
| 📊 Matplotlib | Base visualization library |
| 🎨 Seaborn | Statistical visualization |
| 🤖 Scikit-learn | Machine Learning models & evaluation |
| 📓 Jupyter Notebook | Development environment |

---

## 📁 Dataset Details

| Property | Value |
|----------|-------|
| 📌 Source | Kaggle — Student Performance Dataset |
| 📏 Records | 395 student records |
| 📋 Features | 33 columns |
| 🎯 Target | Pass/Fail (based on G3 >= 10) |

---

## 📂 Project Structure
```
📦 student-performance-analysis-and-prediction
 ┣ 📓 Student_Performance_Analysis.ipynb  → Complete analysis & ML notebook
 ┣ 📊 student-mat.csv                     → Raw dataset
 ┗ 📄 README.md                           → Project documentation
```

---

## 🚀 How to Run
1. Clone this repository
```
git clone https://github.com/Prabha-Jeyaraj/student-performance-analysis-and-prediction.git
```
2. Install required libraries
```
pip install pandas matplotlib seaborn scikit-learn jupyter
```
3. Open notebook
```
jupyter notebook Student_Performance_Analysis.ipynb
```
4. Run all cells and explore! 🎉

---

## 👩‍💻 Author
**Prabha Jeyaraj**
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue)](https://linkedin.com/in/prabhajayaraj09)
