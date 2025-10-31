# 🧮 Employee Salary Analysis and Visualization using Python

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Pandas](https://img.shields.io/badge/Library-Pandas-green)
![Seaborn](https://img.shields.io/badge/Visualization-Seaborn-orange)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)

---

## 📘 Overview
This project performs a **comprehensive data analytics and visualization study** on employee salary information.  
Using **Python, Pandas, Seaborn, and Statsmodels**, it explores how **education level, job title, experience, and gender** influence salary levels within an organization.  
The analysis includes **data cleaning, statistical modeling (ANOVA), and visualization** to uncover key salary trends that can guide **HR policy and compensation strategy**.

---

## 🎯 Objectives
The main goals of this project are to:

1. Analyze salary distributions across job titles, departments, and education levels.  
2. Identify factors that influence salary variations among employees.  
3. Use statistical analysis (ANOVA) to validate the impact of work experience and education on salaries.  
4. Visualize correlations and relationships among variables to gain insights.  
5. Suggest actionable recommendations to improve salary fairness and hiring policies.

---

## 🗂️ Dataset Description

**File Name:** `employee_salary_data.csv`  
**Records:** ~500 employees  
**Columns:**  

| Column Name | Description |
|--------------|-------------|
| Employee_ID | Unique identifier for each employee |
| Job_Title | Role or designation (Engineer, Manager, etc.) |
| Department | Department of the employee |
| Education_Level | Highest level of education (Diploma, Bachelor, Master, PhD) |
| Work_Experience | Total years of experience |
| Monthly_Salary | Current monthly pay |
| Gender | Employee gender |
| Remote_Work_Percentage | % of time spent working remotely |
| Performance_Score | Evaluation of employee performance |

---

## 🧠 Data Preparation & Cleaning
Before analysis, several preprocessing steps were performed:

- Removed missing and duplicate values.  
- Converted categorical variables into numeric dummy variables.  
- Handled outliers in `Monthly_Salary` using the IQR method.  
- Standardized column names for consistency.  
- Ordered categorical variables such as `Education_Level`  
  *(Diploma → Bachelor → Master → PhD)*.

---

## 📊 Exploratory Data Analysis (EDA)
### 1️⃣ Average Salary per Department
Visualized using a **bar plot** to compare average salaries across different departments.  
Departments like **IT** and **Marketing** showed the highest pay levels.

### 2️⃣ Education Level vs Salary
A **line plot** demonstrated a positive trend — employees with higher education (PhD, Master’s) earned more on average.

### 3️⃣ Experience vs Salary
A **scatter plot** was used to visualize the relationship between work experience and monthly salary.  
The result showed a **moderate positive correlation**, confirming that salary increases with experience.

### 4️⃣ Gender and Salary
The analysis found **minor differences** between male and female salaries, indicating relatively fair pay distribution.

### 5️⃣ Salary Distribution by Job Title
A **box plot** illustrated the spread of salaries within each job title.  
Managers and Data Scientists had the **widest and highest ranges**.

### 6️⃣ Correlation Heatmap
A **heatmap** was generated to visualize relationships among numeric variables.  
Education level, experience, and performance were found to have the strongest correlations with salary.

---

## 📊 Statistical Analysis (ANOVA)
The **ANOVA (Analysis of Variance)** test was conducted to determine whether:

| Test | Null Hypothesis | Result |
|------|----------------|--------|
| Work Experience vs Salary | Work experience does not affect salary | ❌ Rejected |
| Education Level vs Salary | Education level does not affect salary | ❌ Rejected |
| Interaction Effect (Education × Experience) | No interaction between education and experience | ❌ Rejected |

📈 **Conclusion:**  
Both **education** and **experience** significantly influence employee salary, and their **interaction** further amplifies this effect.

---

## 💡 Key Insights & Recommendations
- 🎓 Employees with higher education tend to receive higher salaries.  
- 💼 Work experience shows a clear positive effect on salary growth.  
- 🧑‍💻 Departments like **IT** and **Marketing** have higher pay scales.  
- ⚖️ Gender-based salary differences are minimal, showing good equity.  
- 🏠 Employees with higher remote work percentages had slightly lower salaries — possibly due to job nature.  
- 📊 HR can use these insights to develop fairer pay structures and improve hiring decisions.

---

## 🧩 Technologies Used
| Category | Tools |
|-----------|-------|
| Programming Language | Python 3 |
| Data Analysis | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Statistics | Statsmodels (ANOVA, OLS) |
| IDE | Jupyter Notebook |
| Version Control | Git & GitHub |
