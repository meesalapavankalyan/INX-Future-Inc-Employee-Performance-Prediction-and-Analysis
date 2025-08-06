# INX-Future-Inc.-Employee-Performance-Prediction-and-Analysis

---

## 🔍 Project Objectives

- Identify and fix issues in employee performance dataset.
- Understand key drivers of performance.
- Visualize department-wise, gender-wise, and salary-based trends.
- Train ML model to predict future employee performance.
- Build a reusable prediction pipeline.

---

## 🧪 Notebooks Explained

| Notebook                         | Purpose |
|----------------------------------|---------|
| data_processing.ipynb          | Loads raw data, handles missing values, encodes categorical features, and scales data. |
| data_exploratory_analysis.ipynb| Performs detailed EDA using plots (distribution, correlation, department trends). |
| train_model.ipynb              | Trains models (e.g., Random Forest), evaluates accuracy, and saves the best model (employee_perf_rf_model.pkl). |
| predict_model.ipynb            | Loads saved model and predicts performance on new/real-time employee data. |
| visualize.ipynb                | Shows dashboards using Seaborn/Matplotlib for department-wise, experience-wise insights. |

---

## 📦 Model Artifacts

Saved inside: models/saved/

- employee_perf_rf_model.pkl – Trained Random Forest model
- required_features.pkl – List of input features expected by model

---

---

## 🎯 Objective

To develop a predictive analytics solution that classifies employee performance based on historical data. This project helps HR departments identify high or low-performing employees, enabling proactive decisions on promotions, training, or intervention.

---

## 📌 Problem Statement

*INX Future Inc.* is facing challenges in evaluating employee performance objectively across departments. The current manual evaluation process is biased and inconsistent. They provided a dataset containing employee attributes and performance tags and requested a data-driven solution.

---

## 📊 Dataset

- *Source*: Provided by INX Future Inc.
- *Size*: ~3000+ records
- *Target Variable*: PerformanceRating
- *Important Features*:
  - Age
  - Gender
  - Education Background
  - Department
  - Job Role
  - Overtime
  - Total Experience
  - Relationship Satisfaction
  - Training in Last Year
  - Years With Current Manager

---

## 🔍 Notebooks Breakdown

### 1. 📘 data_processing.ipynb
- Loads the raw data
- Handles missing values
- Encodes categorical variables
- Feature selection & scaling
- Saves the processed data into processed/ folder

### 2. 📘 data_exploratory_analysis.ipynb
- Visualizes data distributions
- Performs correlation analysis
- Compares categorical feature impacts
- Plots histograms, boxplots, and heatmaps

### 3. 📘 train_model.ipynb
- Imports processed data
- Splits into train and test sets
- Trains multiple ML models (Random Forest, Logistic Regression, etc.)
- Compares performance with accuracy, precision, recall, F1 score
- Saves best model as employee_perf_rf_model.pkl
- Saves required_features.pkl list for later use

### 4. 📘 predict_model.ipynb
- Loads saved model and required features
- Loads new unseen data
- Predicts employee performance categories
- Exports results to Excel or CSV

### 5. 📘 visualize.ipynb
- Plots final insights
- Bar chart of department-wise performance
- Heatmap for feature impact
- Visualization of prediction vs actual (confusion matrix, classification report)

---

## ✅ Features Used in Model

```python
['Age', 'Gender', 'EducationBackground', 'MaritalStatus', 'EmpDepartment', 
 'EmpJobRole', 'BusinessTravelFrequency', 'DistanceFromHome', 'EmpEducationLevel',
 'EmpEnvironmentSatisfaction', 'EmpHourlyRate', 'EmpJobInvolvement', 'EmpJobLevel',
 'EmpJobSatisfaction', 'NumCompaniesWorked', 'OverTime', 'EmpLastSalaryHikePercent',
 'EmpRelationshipSatisfaction', 'TotalWorkExperienceInYears', 'TrainingTimesLastYear',
 'EmpWorkLifeBalance', 'ExperienceYearsAtThisCompany', 'ExperienceYearsInCurrentRole',
 'YearsSinceLastPromotion', 'YearsWithCurrManager', 'Attrition', 'EmpNumber']


## ▶ How to Run

1. Clone this repo or download the files.
2. Open each .ipynb notebook in Jupyter or VS Code.
3. Run data_processing.ipynb → EDA → train_model.ipynb
4. Make sure models/saved/ folder contains the saved model.
5. Use predict_model.ipynb to load the model and test on new data.

---

## 📊 Tech Stack

- Python
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn
- Jupyter Notebook

---

## 📌 Example Use Case

> Predict whether a newly hired employee is likely to underperform, based on department, education, KPIs, and experience.

---


This project is for academic and learning purposes.
