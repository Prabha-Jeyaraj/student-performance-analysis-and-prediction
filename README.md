# 🎓 Student Performance Analysis & Prediction
> Analyzing student academic performance and predicting pass/fail outcomes using Machine Learning
Show Image Show Image Show Image Show Image

📌 Overview
This project analyzes a real-world student dataset containing 395 student records to identify key factors affecting academic performance and builds a Machine Learning model to predict whether a student will pass or fail their final exam using 13 meaningful features.

📊 Part 1 — Exploratory Data Analysis
📈 Grade Distribution

Analyzed final grade (G3) distribution across all 395 students
Average final grade: 10.42 / 20
265 students passed (67%) and 130 students failed (33%)

📚 Study Time vs Final Grade

Students with higher study time scored significantly better
Clear positive trend — more study time = higher grades
Boxplot used to visualize grade spread across study groups

❌ Past Failures vs Final Grade

Students with no past failures scored highest (median ~12)
Clear negative trend — more failures = lower final grade
Past failures identified as strongest negative factor

🗺️ Correlation Heatmap

Analyzed relationships between all 16 numerical features
G1 (0.90) and G2 (0.80) are strongest predictors of final grade
Past failures showed strongest negative correlation (-0.36) with G3


🤖 Part 2 — Machine Learning
🔧 Data Preparation

Selected 13 meaningful features based on correlation analysis
Encoded categorical columns (higher, internet, romantic) using Label Encoding
Split data: 80% training (316 students) and 20% testing (79 students)
Used stratified split to maintain Pass/Fail ratio in both sets

🏆 Model Results
ModelAccuracyCorrect PredictionsWrong Predictions🥇 Logistic Regression89%70 / 799 / 79🥈 Decision Tree86%68 / 7911 / 79
📋 Logistic Regression — Confusion Matrix
              Predicted Fail    Predicted Pass
Actual Fail        25                1
Actual Pass         8               45
📋 Decision Tree — Confusion Matrix
              Predicted Fail    Predicted Pass
Actual Fail        24                2
Actual Pass         9               44

🔍 Key Findings
✅ G1 and G2 grades are the strongest predictors of final performance
✅ Students with zero past failures perform significantly better
✅ Higher study time consistently leads to better final grades
✅ Logistic Regression outperformed Decision Tree with 89% accuracy
✅ Social factors like going out and alcohol consumption negatively impact grades

🛠️ Tools & Libraries
ToolPurpose🐍 Python 3.13Core programming language🐼 PandasData cleaning & transformation📊 MatplotlibBase visualization library🎨 SeabornStatistical visualization🤖 Scikit-learnMachine Learning models & evaluation📓 Jupyter NotebookDevelopment environment

📁 Dataset Details
PropertyValue📌 SourceKaggle — Student Performance Dataset📏 Records395 student records📋 Features33 columns🎯 TargetPass/Fail (based on G3 >= 10)

📂 Project Structure
📦 student-performance-analysis-and-prediction
 ┣ 📓 Student_Performance_Analysis.ipynb  → Complete analysis & ML notebook
 ┣ 📊 student-mat.csv                     → Raw dataset
 ┗ 📄 README.md                           → Project documentation

🚀 How to Run

Clone this repository

git clone https://github.com/Prabha-Jeyaraj/student-performance-analysis-and-prediction.git

Install required libraries

pip install pandas matplotlib seaborn scikit-learn jupyter

Open notebook

jupyter notebook Student_Performance_Analysis.ipynb

Run all cells and explore! 🎉


👩‍💻 Author
Prabha Jeyaraj
Show Image
