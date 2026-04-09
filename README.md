
# Pandas Data Analysis: Custom & Titanic Datasets

This project demonstrates core **Pandas** data manipulation skills across two parts: building a foundation with a custom dataset and performing exploratory data analysis (EDA) on the Titanic survival dataset.

## 🚀 Overview

- **Part 1:** Creation of a custom Habesha Student Dataset using Python dictionaries.
- **Part 2:** Comprehensive cleaning and analysis of the Titanic `train.csv`.

---

## 🛠️ Part 1: Custom Dataset Foundation
A synthetic dataset was built to practice manual DataFrame construction and custom indexing.

- **Data Structure:** 15 rows × 5 columns.
- **Naming Convention:** Uses Habesha mock names (Given Name + Father's Name).
- **Key Features:** `Name`, `ID`, `City`, `Profession`, `Status`.
- **Implementation:** 
  - Constructed via `pd.DataFrame()` from a Python dictionary.
  - Assigned a custom `MEM_00X` index to simulate unique database IDs.

---

## 🚢 Part 2: Titanic Real-World Analysis
A deep dive into the Titanic passenger list to identify survival patterns through data cleaning and grouping.

### 1. Data Exploration
- Used `.head()` for a quick look at the raw data.
- Used `.info()` and `.isnull().sum()` to identify missing values.
- Used `.describe()` for statistical distribution (Mean, Median, Std).

### 2. Data Cleaning
- **Missing Values:** 
  - `Age`: Imputed using the **median**.
  - `Embarked`: Imputed using the **mode**.
  - `Cabin`: **Dropped** the column due to excessive missing data.
- **Duplicates:** Performed `.drop_duplicates()` to ensure data integrity.

### 3. Insights & Analysis
- **Gender Priority:** Females were significantly more likely to survive than males.
- **Class Impact:** 1st Class passengers had a much higher survival rate compared to 3rd Class.
- **Age Prioritization:** Children (Ages <12) were prioritized during the evacuation.
- **Highest Probability:** The combination of **Female + 1st Class** yielded the highest survival rate.

---

## 💻 Tech Stack
- **Language:** Python 3.x
- **Library:** Pandas

## 📝 How to Use
1. Clone this repository.
2. Ensure `train.csv` is in the project root.
3. Run the analysis script:
   ```python
   import pandas as pd
   # Run the script to see cleaned data and grouped insights
