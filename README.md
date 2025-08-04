# 📊 Placement Analysis of College Students using Data Cleaning and Visualization Techniques

## 📌 Overview
This mini project focuses on analyzing factors that influence college student placements using a dataset of 10,000 entries. We apply data cleaning techniques such as `fillna()` and `dropna()` to handle missing values and use Python libraries to visualize important trends and relationships.

---

## 🧾 Dataset Description
The dataset contains the following columns:

- **College_ID**: Unique identifier for each student  
- **IQ**: Intelligence Quotient  
- **Prev_Sem_Result**: Previous semester result (percentage)  
- **CGPA**: Cumulative Grade Point Average  
- **Academic_Performance**: Overall academic rating  
- **Internship_Experience**: Internship status (Yes/No)  
- **Extra_Curricular_Score**: Score for extracurricular activities  
- **Communication_Skills**: Soft skills rating  
- **Projects_Completed**: Number of completed projects  
- **Placement**: Placement status (Yes/No)

---

## 🧹 Data Cleaning Techniques Used

- `df.dropna()` — Removes rows with any missing values.
- `df.fillna()` — Fills missing numeric values using statistical techniques:
  ```python
  df['Prev_Sem_Result'] = df['Prev_Sem_Result'].fillna(df['Prev_Sem_Result'].mean())
  df['CGPA'] = df['CGPA'].fillna(df['CGPA'].median())
