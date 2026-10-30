# Project Report: Retail Sales Performance Analysis

### Project Details
* **Project Title:** Retail Sales Performance Analysis
* **Project ID:** DA-011
* **Project Domain:** Retail & Sales
* **Current Status:** Completed (Analysis, Visualizations & Insights Finalized)

---

## Project Description
This project looks at store sales data to help businesses make smart choices. It focuses on three main areas:

* **Sales Trends:** Track how much money the store makes each day, month, and 3-month period.
* **Best and Worst Products:** Find out which items sell fast and which ones sell slowly.
* **Customer Shopping Habits:** See how often customers shop, how much they buy at one time, and how they pay.

---

## Methodology & System Architecture

### 1. Step-by-Step Project Approach
To ensure our findings are reliable and reproducible, our team followed a practical 5-step pipeline:

```
[Raw CSV Data] 
       │
       ▼
[Step 1: Data Cleaning] ────> Remove nulls, fix date formats, handle duplicate rows
       │
       ▼
[Step 2: Metric Computation] ─> Calculate Gross Revenue, Order Volumes, Average Bill
       │
       ▼
[Step 3: Visual Analytics] ───> Generate time-series plots, category bar charts
       │
       ▼
[Step 4: Business Insights] ──> Suggest inventory changes & promotion timing
```

1. **Data Collection & Ingestion:** We load transaction records stored in CSV format into Python using Pandas dataframes.
2. **Data Cleaning & Validation:** Raw records usually have empty cells, wrong data types, or duplicate bills. We validate every column before calculating anything.
3. **Exploratory Data Analysis (EDA):** We group records by month, category, and store location to see patterns that are invisible in raw spreadsheets.
4. **Data Visualization:** We convert raw numbers into readable visual charts (bar charts, line graphs) so non-technical managers can understand them immediately.
5. **Actionable Recommendations:** We conclude with clear suggestions, such as which products to restock before peak sales periods.

---

## Technology Used

| Technology / Tool | Type | Description |
| :--- | :--- | :--- |
| **Python** | Programming Language | The core language that powers the entire data pipeline and handles code execution. |
| **Jupyter Notebook** | Interactive Environment | An open-source web application used for creating and sharing documents that contain live code, equations, visualizations, and narrative text. |
| **Google Colab** | Cloud Notebook Environment | A hosted Jupyter notebook service provided by Google that runs entirely in the cloud with free access to computing resources. |
| **Pandas** | Python Library | Used for loading, cleaning, and manipulating tabular data (similar to Excel spreadsheets). |
| **NumPy** | Python Library | Handles large arrays of numbers and performs fast mathematical calculations behind the scenes. |
| **Matplotlib** | Visualization Libraries | Used to generate charts, graphs, and visual reports to easily spot business trends. |
| **CSV** | File Format | The raw data format used to store tabular text data before analysis. |

---

## Implementation & Repository Structure

### Repository Structure
```
Retail-Sales-Performance-Analysis/
│
├── data.csv                 
├── analysis.ipynb          
├── readme.md               
├── requirment.txt         
└── summary.pdf            
```

### Execution & Data Processing Summary

| Pipeline Stage | Implementation Details | Status |
|---|---|---|
| **Data Ingestion** | Loaded 1,545 transaction rows from `data.csv` using Pandas. | **Completed** |
| **Data Cleaning** | Dropped 45 duplicate rows, filled 78 missing prices using product median price. | **Completed** |
| **Field Engineering** | Added `Total_Sales` (Quantity × Unit_Price) and extracted `Transaction_Month`. | **Completed** |
| **Core Visualizations** | Generated 4 essential charts: Monthly Trend, Product Revenue, Category Sales, Location Sales. | **Completed** |

### Summary of Calculated Store Metrics
* **Total Store Revenue:** ₹1,101,336.28
* **Total Completed Orders:** 1,500 transactions
* **Total Physical Units Sold:** 3,682 items
* **Average Order Spend:** ₹734.22 per purchase

---

## Key Findings & Business Recommendations

### 1. Key Analytical Findings
* **Sales Trends Over Time:** Store revenue remained strong across Q1 and Q2, with peak sales in **May (₹152,812)** and **June (₹146,898)**. Weekly shopping traffic was steady across all business days.
* **Best & Worst Selling Products:** The **Pro Gaming Laptop** is the single largest revenue driver, generating **₹653,895** (over **59%** of total store revenue) due to its high unit price. Items like **Plant Protein Powder (₹15,995)** and **Vitamin C Serum (₹20,340)** generated lower revenue despite healthy unit volumes.
* **Category & Store Performance:** **Electronics** leads all categories with **67.7%** of total revenue. Across city branches, **Hyderabad (₹249,036)** and **Chennai (₹228,471)** are top performers, while Bangalore recorded the lowest sales.

### 2. Practical Business Recommendations
1. **Protect and Stock High-Value Inventory:** Ensure high-demand electronics like laptops remain safely stored and consistently in stock, as they generate the vast majority of revenue.
2. **Introduce Product Bundles:** Pair lower-priced, high-volume items (skincare serums and health supplements) with apparel or tech accessories to increase average order spend.
3. **Targeted Regional Promotions:** Run localized discounts and marketing campaigns in Bangalore and Delhi to help those stores reach the revenue levels of Hyderabad and Chennai.

### 3. Project Conclusion
All project objectives for **DA-011** have been completed. Raw transactions were cleaned, key store KPIs were calculated, and the four essential visual charts were generated. The findings provide clear, practical guidance for retail inventory management and sales strategy.

---

## Project Links

| Type | Link |
| :--- | :--- |
| **GitHub Repository** | [GitHub Repo](https://github.com/Sami-Last-Breath-Programming/Retail-Sales-Performance-Analysis) |
| **Jupyter Notebook** | [analysis.ipynb](analysis.ipynb) |
| **Raw Dataset** | [data.csv](data.csv) |
| **Colab Notebook Link** | [Analysis Notebook](https://colab.research.google.com/drive/1pNdqqJyovQdowKETfQJsCBiMxADcmyNK?usp=sharing) |

---

## References 

| Technology | Reference |
| :--- | :--- |
| **Python** | [Python Official Documentation](https://docs.python.org/) |
| **Jupyter Notebook** | [Jupyter Documentation](https://docs.jupyter.org/) |
| **Google Colab** | [Google Colab Portal](https://developers.google.com/colab) |
| **Pandas** | [Pandas PyPI / Documentation](https://pypi.org/project/pandas/) |
| **NumPy** | [NumPy Documentation](https://numpy.org/doc/stable/) |
| **Matplotlib** | [Matplotlib Documentation](https://matplotlib.org/stable/index.html) |
| **Seaborn** | [Seaborn Documentation](https://seaborn.pydata.org/) |
| **CSV** | [Python CSV Library Documentation](https://docs.python.org/3/library/csv.html) |

---

## Project Members

| Name | ID |
| --- | --- |
| **NIDA** | BCAI2026011 |
| **ABDUL SAMI** | BCAI2026010 |
| **SIYA GUPTA** | BCAI2026009 |
| **AYUSH SINGH** | BCAI2026004 |
| **LAXMI JOSHI** | BCAI2026006 |
| **ARJUN SHARMA** | BCAI2026002 |
| **AYUSH SHARMA** | BCAI2026007 |
| **KOMAL KUMARI** | BCAI2026013 |
| **PARAS GANGWAR** | BCAI2026001 |
| **MANISHA TIWARI** | BCAI2026005 |
| **SHARANYA SINGH** | BCAI2026008 |
| **MANISH RAJ SINGH** | BCAI2026015 |
| **NIRBHAY RAJ SINGH** | BCAI2026003 |
| **ADITYA PRIYANSHU VERMA** | BCAI2026012 |
