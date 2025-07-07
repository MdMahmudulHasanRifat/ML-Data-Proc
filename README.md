# Diabetes Prediction using Linear Regression

## 📘 Overview
This project predicts whether a patient has diabetes using a Linear Regression model. Although Linear Regression is typically used for continuous outputs, we apply rounding to get binary predictions (0 or 1), enabling classification.

## 📁 Dataset
- **File Name**: `diabetes.csv`
- **Source**: [PIMA Indians Diabetes Dataset](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)
- **Used from GitHub**:  
  [Raw CSV Link](https://raw.githubusercontent.com/MdMahmudulHasanRifat/ML-Data-Proc/refs/heads/main/diabetes.csv)

## 🧹 Preprocessing Steps
1. Replaced zero values in the following columns with the **column mean**:
   - Glucose
   - BloodPressure
   - SkinThickness
   - Insulin
   - BMI
2. Set the **first row's glucose value** to the **maximum glucose** in the column.
3. Found the **minimum age**, and replaced glucose values of those records with the **minimum glucose**.

## 🧠 Modeling
- **Model Used**: Linear Regression (`sklearn.linear_model.LinearRegression`)
- **Output**: Continuous predictions were rounded to `0` or `1` for classification.

## 🧪 Evaluation Metrics
| Metric     | Result (Example) |
|------------|------------------|
| Accuracy   | 0.77             |
| Precision  | 0.73             |
| Recall     | 0.56             |
| F1 Score   | 0.63             |

- **Confusion Matrix** is also plotted using seaborn.

## ▶️ How to Run
1. Open the notebook in Google Colab or Jupyter.
2. Make sure `pandas`, `numpy`, `matplotlib`, `seaborn`, and `scikit-learn` are installed.
3. No need to upload CSV manually — the dataset is loaded directly from GitHub.
4. Run all cells to see predictions and evaluation metrics.

## 📌 Notes
- Linear Regression is not ideal for binary classification, but this was used as per lab instructions.
- For improved results, models like **Logistic Regression** or **Random Forest** are recommended.

---

✅ **Author**: Md Mahmudul Hasan Rifat
🆔 **Student ID**: 222002048  
📘 **Course**: CSE312 - Section 222D3  
📝 **Lab Report 01**
