# Task 21 — Missing Value Analysis Using Pandas

## Project Overview

This project identifies missing values in a student performance dataset using Python and Pandas.

It calculates column-wise missing-value counts and percentages, identifies incomplete records, and determines which columns require further treatment.

## Objectives

- Identify missing values using `isnull()` and `isna()`.
- Calculate missing-value counts for each column.
- Calculate the percentage of missing values.
- Create a missing-value summary.
- Identify columns requiring treatment.
- Examine records containing missing values.

## Technologies Used

- Python
- Pandas
- NumPy
- Google Colab
- Jupyter Notebook

## Dataset Description

The project uses a manually created student performance dataset containing 12 fictional records and six columns:

- Student ID
- Name
- Department
- Age
- Marks
- Attendance

Intentional missing values are included in the department, age, marks, and attendance columns.

## Pandas Functions Used

- `df.isnull()` — identifies missing values.
- `df.isna()` — provides another method of identifying missing values.
- `df.sum()` — calculates column-wise missing counts.
- `df.mean()` — used to calculate missing-value percentages through Boolean values.
- `df.size` — returns the total number of cells.
- `df.isnull().any(axis=1)` — identifies rows containing missing values.

## Key Results

| Column | Missing Values | Missing Percentage |
|---|---:|---:|
| student_id | 0 | 0% |
| name | 0 | 0% |
| department | 1 | 8.33% |
| age | 1 | 8.33% |
| marks | 2 | 16.67% |
| attendance | 2 | 16.67% |

Total missing cells: 6

Columns requiring treatment: department, age, marks, attendance.

## Treatment Recommendations

- Department: Mode imputation or an Unknown category.
- Age: Median imputation.
- Marks: Median imputation.
- Attendance: Median imputation.

These are recommendations only; the original dataset is not modified.

## Project Files

- `Task_21_Missing_Value_Analysis.ipynb` — Google Colab notebook.
- `missing_values_dataset.csv` — Input dataset.
- `missing_value_summary.csv` — Column-wise missing-value summary.
- `requirements.txt` — Required libraries.
- `README.md` — Project documentation.
- `project_report.pdf` — Formal project report.
- `screenshots/` — Execution evidence.

## Conclusion

This project demonstrates how Pandas can identify missing values, calculate missing-value percentages, and highlight columns requiring treatment.

These techniques are important for data cleaning and preparing reliable datasets for machine learning.
