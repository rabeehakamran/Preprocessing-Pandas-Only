#  Sales Data Cleaning & Analysis (Pandas)

This project demonstrates **data cleaning, preprocessing, feature engineering, and querying** using **Pandas** on `Sales_Data.csv`.

---

## 📌 Steps

### 1. Data Loading & Inspection
- Load dataset with Pandas.
- Check dimensions, datatypes, summary stats, and missing values.

### 2. Data Cleaning
- Fill missing values:
  - Numeric → median  
  - Categorical → mode / "Unknown"  
  - Address/Phone → defaults
- Convert `ORDERDATE` to datetime → extract `QTR_ID`, `MONTH_ID`, `YEAR_ID`.
- Create `SALES = QUANTITYORDERED × PRICEEACH`.
- Drop high-null columns (`ADDRESSLINE2`, `STATE`, `POSTALCODE`, `TERRITORY`, `MSRP`).
- Remove duplicates.

### 3. Feature Engineering
- Add `TOTALPRICE`, `MONTH`, `DAY`, `HOUR`.
- Clean `CITY` & `COUNTRY` strings.

### 4. Querying
- All orders of **Trucks & Buses**.  
- Orders in **January**.  
- **High-value orders** (`TOTALPRICE > 500`).  

---

## 🛠 Libraries
- `pandas`  
- `numpy`  

---

## 📊 Example Outputs
- Unique Product Lines: `['motorcycles','classic cars','trucks and buses','vintage cars','planes','ships','trains']`
- High Price Orders (>500): sample → `ORDERNUMBER=10107 | TOTALPRICE=2871 | CITY=NYC | COUNTRY=USA`

---

✅ Cleaned & analysis-ready dataset with meaningful insights.
