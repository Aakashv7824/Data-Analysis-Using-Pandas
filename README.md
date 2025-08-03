# Heart Disease Exploratory Analysis

A self-contained Jupyter Notebook that walks through an end-to-end exploratory data analysis (EDA) of U.S. heart disease datasets from 2020 and 2022. This project demonstrates best practices in data cleaning, profiling, visualization, metric derivation, and export—making it a ready-to-share template for cardiovascular risk analysis.

---

---

## 📝 Notebook Overview

1. **Data Loading**  
   - Reads three CSV files (`heart_2020_cleaned.csv`, `heart_2022_no_nans.csv`, `heart_2022_with_nans.csv`) into Pandas DataFrames.  

2. **Data Cleaning**  
   - Applies a reusable `clean_dataframe()` function to each DataFrame:  
     - Standardizes column names to snake_case  
     - Fills missing values with median (numerical) or mode (categorical)  
     - Converts data types (e.g., dates, numeric flags)  
     - Drops exact duplicates  

3. **Data Profiling**  
   - Computes summary statistics (`.describe()`) and value counts for key features:  
     - Demographics: age group, sex, race/ethnicity, state  
     - Clinical factors: cholesterol level, blood pressure, smoking status, diabetes  

4. **Data Visualization**  
   - Uses Matplotlib to plot:  
     - Distribution of smoking and diabetes status  
     - Bar charts of heart attack incidence by age group, gender, ethnicity, and state  
     - Correlation heatmap of continuous risk factors  

5. **Metrics Derivation**  
   - Identifies top demographic segments with highest heart disease rates  
   - Calculates relative risk ratios for key predictors  
   - Summarizes five actionable KPIs (e.g., “Age 65+ smokers have X× higher incidence”)  

6. **Export**  
   - Saves the fully cleaned and imputed master DataFrame to `heart_disease_cleaned_master.csv` for downstream modeling or reporting.

---

## 🛠️ Setup & Dependencies

- **Python 3.8+**  
- **Key libraries:**  
  ```bash
  pandas
  matplotlib
  seaborn
  numpy


