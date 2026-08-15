# 🛒 Plug & Play E-commerce Profitability Engine

##  Project Overview
This project is an amateur automated Business Intelligence engine built in Power BI, designed for e-commerce store owners (Shopify/WooCommerce). It transforms raw, messy exports of sales and marketing data into a clean Star Schema, calculating true net profitability, CAC, and LTV without the need for expensive ETL SaaS middleware.

##  Architecture & Tech Stack
* **Power BI / DAX:** Core analytical engine and dynamic measures.
* **Power Query (M Code):** Advanced automated ETL process featuring dynamic folder ingestion, error handling, and `en-US` culture locking.
* **Python:** Used to generate 600+ rows of synthetic relational data (Orders, Products, Marketing).

##  The Problem it Solves
Most e-commerce owners struggle with "Data Granularity Mismatch" – sales happen at the order-line level, while marketing spend happens at the daily-campaign level. This engine uses a dynamic ETL process to bridge this gap automatically.

##  Core Features (KPIs)
- **Net Margin Waterfall:** From Gross Revenue down to True Profit.
- **CAC & ROAS Tracking:** Marketing spend mapped against returning vs. new customers.
- **Automated Data Cleaning:** Built-in safeguards for incorrect data inputs.

##  How to Use (Synthetic Data Demo)
1. Download the `Test_1` from the `/data` folder.
2. Open the `.pbip` project in Power BI Desktop.
3. Update the `FolderPath` parameter to point to your local data folder.
4. Refresh and explore the dashboard!