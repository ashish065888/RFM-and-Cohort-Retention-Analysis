# RFM-and-Cohort-Retention-Analysis

## Project Overview
An end-to-end data analysis project that answers:

> **Which customers and products drive repeat revenue, and how can the business improve retention?**

This project analyzes transactional data from a UK-based online retailer to understand customer behavior, product performance, and repeat-purchase patterns.


## Business Problem

The business wants to know:

- Who are the most valuable customers?
- Which customers are likely to buy again?
- Which products are associated with repeat purchases?
- How can the business increase repeat revenue and average order value?

The goal is to turn raw transactions into actionable insights for marketing, retention, and product strategy.

## Dataset

**Source:** [UCI Online Retail Dataset](https://archive.ics.uci.edu/dataset/352/online+retail)

- Real transactional data from a UK-based online retailer.
- Contains invoice-level transactions with product, quantity, price, date, customer, and country information.
- Time period: December 2010 to December 2011.
- Approximately 541,909 transactions and 8 columns. [142][147]

### Key columns used
| Column | Description |
|---|---|
| `InvoiceNo` | 6-digit transaction ID. Codes starting with "C" mean a cancellation. |
| `StockCode` | 5-digit product ID. |
| `Description` | Product name |
| `Quantity` | Number of units purchased |
| `InvoiceDate` | Date and time of transaction |
| `UnitPrice` | Price per unit in British Pounds (£) |
| `CustomerID` | 5-digit unique customer ID |
| `Country` | Customer country |


## Tools Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Data Cleaning and Preprocessing
The following data cleaning operations were performed:
1. Rows with missing CustomerIDs are removed.
2. Identified and removed duplicate rows.
3. Removed cancelled invoices.
4. Checked each column for mixed data types and corrected wherever needed.
5. Resolved inconsistent description (extra spaces, commas, and abbreviations) by mapping all variations to a single standardized name based on StockCode and Description renamed to ProductName.

## Key Analysis Sections

### Sales Performance

