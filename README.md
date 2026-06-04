🎓 Student Performance Prediction using Machine Learning

📌 Overview

This project aims to predict students' final grades (G3) using demographic, academic, and lifestyle features.

The goal is to explore how different machine learning models perform on real-world educational data and identify the most influential factors affecting student performance.

---

🎯 Objectives

- Build and compare multiple regression models
- Understand the impact of different features on student performance
- Evaluate model performance using R² score
- Apply a complete machine learning workflow from data preprocessing to evaluation

---

📊 Dataset

- Source: UCI Machine Learning Repository
- Records: 395 students
- Features: 30+ attributes including:
  - Academic (study time, failures)
  - Social (going out, relationships)
  - Personal (age, health)

---

⚠️ Important Note: Data Leakage

Features G1 and G2 (previous grades) were removed to avoid data leakage.

Including these features would lead to unrealistically high model performance, as they are strongly correlated with the final grade (G3).

---

🔄 Data Preprocessing

- Checked for missing values (none found)
- Removed leakage features (G1, G2)
- Applied one-hot encoding to categorical variables
- Split data into training and testing sets

---

🤖 Models Used

Model| Description
Linear Regression| Assumes linear relationship between features and target
Decision Tree| Captures non-linear patterns using tree-based splits
Random Forest| Ensemble model that reduces overfitting and improves performance

---

📈 Model Performance

Model| R² Score
Linear Regression| ~0.20
Decision Tree| ~0.26
Random Forest| ~0.39

---

🧠 Key Insights

- Failures is one of the strongest predictors of final grade
- Absences negatively impact student performance
- Social behavior (goout) shows influence on academic results
- The dataset contains non-linear relationships better captured by tree-based models

---

🔍 Interpretation

- Linear Regression performed poorly due to weak linear relationships in the dataset
- Decision Tree improved performance than Linear Regression by capturing non-linear patterns
- Random Forest outperformed the Linear Regression and  Decision Tree model in this case

Overall performance remains moderate, suggesting that student performance depends on additional factors not fully captured in the dataset.

---

⚠️ Limitations

- Small dataset size (395 samples)
- Missing real-world factors such as motivation, teaching quality, and environment
- Moderate predictive performance

---

🚀 Future Improvements

- Try advanced ensemble models
- Perform feature engineering
- Use cross-validation for more robust evaluation
- Incorporate additional datasets for better predictions

---

🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

---

📌 Conclusion

Random Forest achieved the best performance in this project, demonstrating the importance of capturing non-linear relationships in educational data.

The project highlights that understanding data, preprocessing carefully, and interpreting results are just as important as choosing machine learning models.