# 📘 Multiple Linear Regression – Predicting Exam Score

This project demonstrates the use of **Multiple Linear Regression** to predict students' **Exam Scores** based on several independent features, including **Study Hours** and additional variables.

---

## 📦 Dataset Overview

The dataset used in this notebook is named `StudyHoursWithFeatures.csv` and contains the following features:

| Column Name           | Description |
|------------------------|-------------|
| **Study Hours**        | Number of hours a student studied per day. |
| **Sleep Hours**        | Average hours of sleep the student gets per day. |
| **Attendance Rate**    | Percentage of class attendance (0–100%). |
| **Social Media Hours** | Daily hours spent on social media. |
| **Exam Score**         | Final exam score (target variable to be predicted). |

---

## 🔍 Objective

To build a multiple linear regression model that accurately predicts a student’s exam score based on their study behavior and other related factors.

---

## 🧹 Preprocessing Steps

- **Exploratory Data Analysis (EDA)** using `pairplot` and regression plots
- **Train-test split** with `25%` as the test size
- **Feature scaling** with `StandardScaler` to standardize input variables
- **Model training** using `LinearRegression` from `scikit-learn`

---

## 📈 Evaluation Metrics

The model was evaluated on the test set using the following metrics:

- **Mean Squared Error (MSE)**
- **Mean Absolute Error (MAE)**
- **R² Score** (Coefficient of Determination)
- **Adjusted R² Score**

These metrics provide insight into how well the model generalizes to unseen data.

---

## 📊 Model Insights

- Model coefficients and intercept were extracted to understand the influence of each feature.
- **Residual analysis** was conducted using a KDE (Kernel Density Estimation) plot to check the distribution of errors.
- The residuals were fairly normally distributed, indicating a good fit.

---

## 🛠️ Libraries Used

- `pandas` and `numpy` – Data loading and manipulation  
- `matplotlib` and `seaborn` – Visualization  
- `scikit-learn` – Model training, preprocessing, and evaluation

---

## ▶️ How to Run

1. Make sure you have the dataset `StudyHoursWithFeatures.csv` in your working directory.
2. Install required dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
