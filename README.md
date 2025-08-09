# Indian-Startup-Funding-Analysis

Here’s a README file for your `mainn.py` script:

---

# Startup Funding Data Analysis

## 📌 Overview

This project analyzes startup funding data from `startup_funding.csv`. It performs data cleaning, transformation, aggregation, and visualization to uncover trends such as:

* Funding patterns over time
* Top sectors, cities, startups, and investors
* Popular investment types

The analysis includes both numerical summaries and visualizations.

---

## 📂 Features

1. **Data Loading & Cleaning**

   * Reads CSV file using Pandas
   * Removes unnecessary columns (`Remarks`)
   * Fills missing values with `"Unknown"`
   * Cleans numerical and date formats
   * Standardizes text fields (lowercase, no extra spaces, removes non-ASCII)

2. **Feature Engineering**

   * Extracts `FundingYear` and `FundingMonth` from the funding date

3. **Data Aggregations**

   * Yearly and monthly funding trends
   * Top 10 sectors, cities, and startups by funding
   * Top 10 investors by total funding and number of deals
   * Investment types by funding and deal count

4. **Visualizations**

   * Line plots for funding trends
   * Bar charts for top sectors, cities, startups, investors, and investment types

---

## 🛠 Requirements

Install dependencies using:

```bash
pip install pandas matplotlib seaborn
```

---

## 📜 How to Run

1. Place your `startup_funding.csv` file in the `/content/` directory or update the path in the script.
2. Run the script:

```bash
python mainn.py
```

3. View printed summaries in the console and visualizations in pop-up windows.

---

## 📊 Output

The script produces:

* Data summaries (`.head()` and `.info()`)
* Aggregated funding statistics
* Visualizations for:

  * Yearly funding trends
  * Top sectors, cities, startups
  * Top investors (funding & deals)
  * Top investment types

---

## 📌 Notes

* Ensure your CSV file contains the expected columns:

  * `Sr No`, `Date dd/mm/yyyy`, `Startup Name`, `Industry Vertical`, `SubVertical`,
    `City  Location`, `Investors Name`, `InvestmentnType`, `Amount in USD`, `Remarks`
* Any missing or malformed data is handled gracefully.

---
