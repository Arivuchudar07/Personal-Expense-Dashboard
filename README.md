# Personal Expenses Dashboard

An interactive Power BI dashboard designed to track, analyze, and manage personal finances. This project helps users gain insights into their spending habits, monitor monthly savings rates, and understand cash flow patterns over time.

## 🚀 Features

- **KPI Overview:** Real-time visibility into Total Income, Total Expenses, Net Savings, and Savings Rate percentage.
- **Expense Categorization:** Interactive breakdown of spending across various categories (e.g., Housing, Groceries, Entertainment, Utilities).
- **Monthly Trends:** Line and column charts showcasing historical income vs. expense trends to identify seasonal spikes.
- **Payment Method Analysis:** Insights into preferred modes of transactions (Credit Card, Debit Card, Cash, etc.).
- **Dynamic Filtering:** Slicers for deep-diving into specific years, months, expense types, or categories.

## 🛠️ Built With

- **Power BI Desktop:** For report design, visual building, and dashboard layout.
- **Power Query:** Used for ETL (Extract, Transform, Load) processes—cleaning data, setting data types, and consolidating transaction files.
- **DAX (Data Analysis Expressions):** Utilized for custom measures (e.g., Running Totals, Year-over-Year growth, Expense percentages).

## 🗂️ Data Model Structure

The dashboard follows a **Star Schema** architectural model for optimal performance:
- **Fact Table:** `Fact_Transactions` (Stores all income and expense entries with amounts, dates, and account details).
- **Dimension Tables:** - `Dim_Categories` (Expense/Income categories and sub-categories).
  - `Dim_Calendar` (A custom DAX auto-generated date table for seamless time intelligence functions).
  - `Dim_Accounts` (Payment methods/bank accounts).
