# Task 1: Data Cleaning & Preprocessing
**Internship:** SoftNexis Technology  
**Intern Name:** Shubham Jaiswal  
**Domain:** Data Science & Machine Learning Using Python  
**Intern ID:** SN1001074

---

## Objective
Clean and preprocess a raw customer dataset to make it ready for analysis by handling duplicates, missing values, data type issues, and formatting inconsistencies.

---

## Steps Performed

### 1. Data Ingestion
- Loaded the dataset using `pd.read_csv()`
- Performed initial sanity checks using `df.head()`, `df.info()`, `df.describe()`

### 2. Deduplication
- Checked for duplicate rows using `df.duplicated()`
- Removed duplicates using `df.drop_duplicates()`

### 3. Column Management
- Dropped irrelevant columns: `Index`, `Phone 2`
- Renamed all columns to lowercase with underscores for consistency
- Reordered columns logically

### 4. Missing Value Handling
- Diagnosed missing values using `df.isna().sum()`
- Dataset had no missing values — documented and verified

### 5. Data Type Correction
- Converted `subscription_date` from string to datetime using `pd.to_datetime()`

### 6. Format Standardization
- Standardized `customer_id` to uppercase
- Converted `email` to lowercase
- Applied title case to `first_name`, `last_name`, `city`, `country`
- Stripped extra whitespace from all text columns

---

## Libraries Used
- `pandas`
- `numpy`

---

## Outcome
A clean, analysis-ready dataset saved as `cleaned_customers.csv` with consistent formatting, correct data types, and no duplicates or missing values.
```

---

### Folder structure on GitHub should look like this:
```
SoftNexis-Data-Science-Internship/  
│
└── Task1_Data_Cleaning/
    ├── README.md  
    ├── Task1_Data_Cleaning.ipynb  
    ├── customers-1000.csv  
    └── cleaned_customers.csv 
