Employee Salary Prediction using XGBoost

This project predicts whether an individual's income exceeds $50K per year using demographic and employment data.  
The model is trained on the **Adult Income dataset (Census Income Data)** and built with **XGBoost** in a Scikit-Learn pipeline.

---

Dataset

- **adult.csv**
- **Target Variable**: `income` (`<=50K` or `>50K`)
- **Features** include: age, workclass, education-num, occupation, race, sex, capital-gain/loss, hours-per-week, etc.

---
Project Workflow

1. **Data Cleaning**
   - Removed rows with missing values
   - Dropped redundant `education` column
   - Handled outliers using the IQR method

2. **Feature Engineering**
   - Applied **OneHotEncoding** to categorical variables
   - Kept numeric columns as-is

3. **Model Building**
   - Used **XGBoostClassifier** wrapped in a `Pipeline`
   - Trained with `train_test_split` (80-20)

4. **Evaluation Metrics**
   - Accuracy Score
   - Precision, Recall, F1-score
   - Confusion Matrix Visualization

---

Model Performance (XGBoost)

| Metric      | <=50K | >50K |
|-------------|--------|-------|
| Precision   | ~0.87  | ~0.68 |
| Recall      | ~0.90  | ~0.53 |
| F1-score    | ~0.88  | ~0.59 |

*(Values may vary slightly based on preprocessing)*

---
<img width="691" height="547" alt="one__" src="https://github.com/user-attachments/assets/7a356a85-354a-45cb-a680-9867a0fd253f" />

Files in this Repo

| File | Description |
|------|-------------|
| `employee_salary_prediction.ipynb` | Main notebook with complete pipeline |
| `adult 3.csv` | Cleaned dataset (or assumed to be downloaded at runtime) |
| `README.md` | You're reading it! |

---
<img width="548" height="455" alt="confusion matrix" src="https://github.com/user-attachments/assets/47871535-c6ef-4e4b-8cf1-26a46c5a3c95" />
Precision-Recall Curve:
<img width="691" height="547" alt="precison" src="https://github.com/user-attachments/assets/51fdf4bc-74a0-4527-b789-67b872f71831" />

Tech Stack

- Python 3.x
- Pandas, NumPy, Matplotlib, Seaborn
- Scikit-Learn
- XGBoost
- Google Colab

---
<img width="448" height="455" alt="one__" src="https://github.com/user-attachments/assets/b7bed027-608c-4893-ad42-47cec3e7fe16" />

Future Enhancements

- Apply **SMOTE** or **Class Weights** for better balance
- Compare with other models: Logistic Regression, Random Forest
- Deploy as a simple web app using **Streamlit** or **Flask**

---

Capstone Project

---



