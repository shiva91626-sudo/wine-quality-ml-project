# wine-quality-ml-project
End-to-end ML project: Regression + Classification on Wine Quality Dataset.

📌 Wine Quality Prediction — Regression + Classification

This project explores the Wine Quality Dataset using regression and classification models to understand the chemical factors behind wine quality.

🔍 Project Goals

Predict exact wine quality score (3–9) → Regression

Predict if wine is Good (≥6) or Bad (<6) → Classification

Understand feature importance and model behavior

Build an end-to-end ML workflow for real-world data

📊 Data Overview

6497 samples

11 numeric features

Target: quality score

No missing values

Imbalanced distribution (most wines are quality 5–6)

🧪 Regression Models Tested
| Model             | MAE      | RMSE     | R²       | Notes             |
| ----------------- | -------- | -------- | -------- | ----------------- |
| Linear Regression | 0.56     | 0.74     | 0.26     | Baseline          |
| Ridge             | 0.567    | 0.739    | 0.259    | Similar to linear |
| Lasso             | 0.568    | 0.739    | 0.259    | Similar, simpler  |
| Random Forest     | 0.43     | 0.60     | 0.50     | ⭐ Best           |


Insight: Wine quality is non-linear → Tree models perform better.

🧠 Classification Experiment (Good vs Bad Wine)

Converted target:

1 = Good (≥6)

0 = Bad (<6)

Logistic Regression Results

Accuracy: 73%

F1 (Good): 0.79

F1 (Bad): 0.60

Handles imbalance well and gives strong performance.

🔍 Key Feature Importance (Random Forest)

Alcohol (highest positive impact)

Volatile acidity (negative impact)

Sulphates

Free sulfur dioxide

Total sulfur dioxide

📘 Files in This Repository

notebook/wine_project.ipynb → Full analysis & modeling

reports/Wine_Quality_Project.pdf → Detailed PDF report

README.md → Project summary


🚀 Conclusion

Random Forest is the most effective regression model.

Logistic Regression achieves strong classification results.

Alcohol and volatile acidity dominate wine quality prediction.

This project demonstrates an end-to-end ML pipeline with interpretability and business insights.
