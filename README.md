# Task-1-Rishitha
# Data Analytics Project 1 – Data Cleaning using Python

## Project Overview

This project focuses on performing **data cleaning and preprocessing** on a dataset using Python and Pandas. The objective is to identify missing values, handle incomplete records, and prepare the dataset for further analysis.

---

## Objective

* Load dataset from Excel
* Identify missing values
* Clean missing data
* Replace missing coupon values with a default label
* Save cleaned dataset into a new Excel file

---

## Technologies Used

* Python
* Pandas
* NumPy
* Jupyter Notebook / Google Colab

---

## Dataset

Input file:

`dataset.xlsx`

Output file:

`clean_project1_dataset.xlsx`

---

## Steps Performed

### 1. Import Libraries

```python
import pandas as pd
import numpy as np
```

### 2. Load Dataset

```python
df = pd.read_excel("dataset.xlsx")
```

### 3. Check Missing Values

```python
print(df.isnull().sum())
```

### 4. Handle Missing Values

```python
df['CouponCode'] = df['CouponCode'].fillna("No Coupon")
```

### 5. Save Cleaned Dataset

```python
df.to_excel("clean_project1_dataset.xlsx", index=False)
```

---

## Output

* Missing values identified
* CouponCode column cleaned
* New cleaned Excel dataset generated

---

## Conclusion

This project demonstrates the process of cleaning real-world data using Python. Proper preprocessing improves data quality and makes datasets suitable for analysis and visualization.

---

## Repository Structure

```
Project-1/
│
├── dataset.xlsx
├── DATA ANALYTICS.pdf
├── project1.ipynb
└── README.md

```
