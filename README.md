# fintech_transactions-DATA-ANALYTICS-MINOR-PROJECT
This dataset represents records of 200 financial transactions processed across different countries and merchants in a fintech environment. Each row corresponds to a single transaction made by a customer, including details such as the amount, date, payment method, currency, and transaction status.


# Fintech Transactions Dataset - Cleaned Version

## Overview

This dataset represents 200 simulated fintech transactions made by customers across different countries and merchants. It is designed for data analysis, visualization, and model training purposes related to financial transactions and consumer spending behavior.

The dataset was cleaned to ensure consistency, accuracy, and readiness for analysis.

---

## Data Description

Each record (row) represents a single transaction. The columns include:

| Column Name        | Description                                                                         |
| ------------------ | ----------------------------------------------------------------------------------- |
| **Transaction_ID** | Unique identifier for each transaction (e.g., `T100001`).                           |
| **Customer_Name**  | Name of the customer making the transaction. Cleaned to proper case.                |
| **Date**           | Standardized date of transaction in the format `YYYY-MM-DD`.                        |
| **Amount**         | Numeric transaction value with currency symbols removed.                            |
| **Currency**       | ISO 3-letter currency code (e.g., `USD`, `INR`, `EUR`).                             |
| **Merchant**       | Platform or company where the transaction took place (e.g., Amazon, Zomato, Apple). |
| **Category**       | Type of spending such as `Travel`, `Transport`, or `Utilities`.                     |
| **Payment_Method** | Payment channel used — such as `UPI`, `Debit Card`, or `Bank Transfer`.             |
| **Status**         | Final state of the transaction — `Completed`, `Pending`, `Cancelled`, or `Failed`.  |
| **Country**        | Country associated with the transaction. Standardized to proper title case.         |

---

## Cleaning Process

The dataset underwent several cleaning steps to remove inconsistencies and errors:

1. **Date Standardization**

   * Converted mixed formats like `18/05/2024` and `Jun 15, 2024` to `YYYY-MM-DD`.

2. **Amount Conversion**

   * Removed symbols (like `$`) and textual currency references.
   * Converted all amounts into floating-point numeric values.

3. **Currency Normalization**

   * Extracted valid ISO 3-letter codes only (e.g., from `USD GBP` → `USD`).

4. **Text Standardization**

   * Removed extra spaces and applied proper case to names, merchants, and countries.

5. **Duplicate Removal**

   * Dropped redundant or repeated transaction records.

6. **Integrity Checks**

   * Verified that all numeric and categorical fields are valid and properly typed.

---

## Possible Analyses

This cleaned dataset can be used for:

* **Spending Trend Analysis:** Track spending behavior by category, merchant, or region.
* **Payment Method Insights:** Compare transaction counts and volumes by payment type.
* **Transaction Success Rate:** Measure success vs. failure ratios across merchants or countries.
* **Currency Distribution:** Identify regions or users based on currency usage.
* **Customer Segmentation:** Analyze spending patterns by customer name or region.

---

## Example Insights (Post-Cleaning)

* Highest transaction category: Travel & Transport.
* Most common merchants: Amazon, Zomato, Apple.
* Most used payment methods: Debit Card and UPI.
* Currency distribution primarily includes USD, EUR, INR, and GBP.

---

## Usage

This dataset can be used for:

* Data cleaning and preprocessing exercises.
* Machine learning model training (fraud detection, trend prediction, etc.).
* Visualization projects (Power BI, Tableau, Python Matplotlib/Pandas).
* Educational demonstrations for financial data handling.

---

## License

This dataset is intended for **educational and research purposes only**. It contains synthetic, non-identifiable data.

---

## Author

**Prepared by:** Data Cleaning and Analysis Pipeline (Ronit Shekhar)
**Date:** November 2025
**File Name:** `fintech_transactions_cleaned.csv`
