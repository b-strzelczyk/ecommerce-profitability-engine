# Plug & Play E-commerce Profitability Engine

##  Project Overview
This project is an amateur automated Business Intelligence engine built in Power BI, designed for e-commerce store owners (Shopify/WooCommerce). By utilizing a simple, standardized input template, it transforms your sales and marketing data into a clean Star Schema, calculating true net profitability, CAC, and LTV. Furthermore, it serves as an uncomplicated executive dashboard that is truly "plug & play" — business owners just paste their data into the provided template, click refresh, and make data-driven decisions without needing any technical knowledge of data engineering, Power Query, or DAX.

##  Architecture & Tech Stack
* **Power BI / DAX:** Core analytical engine and dynamic measures.
* **Power Query (M Code):** Automated ETL process equipped with error handling and `en-US` culture locking to ensure data format stability.
* **Python:** Used to generate 600+ rows of synthetic relational data (Orders, Products, Marketing) to populate the demo template.

##  The Problem it Solves
Most e-commerce owners struggle with "Data Granularity Mismatch" – sales happen at the order-line level, while marketing spend happens at the daily-campaign level. This engine bridges this gap automatically once the data is pasted into the template.

##  Core Features (KPIs)
- **Zero-Tech Setup via Template:** Just copy and paste your daily/monthly exports into our ready-made input template. No API configurations or complex pipelines required.
- **Net Margin Waterfall:** From Gross Revenue down to True Profit.
- **CAC & ROAS Tracking:** Marketing spend mapped against returning vs. new customers.
- **Automated Data Processing:** Built-in safeguards in Power Query map the template data correctly into the relational model.

##  How to Use (Synthetic Data Demo)
1. Download the `Ecom_profitability_engine_data_template_v1.0` template from the `/data` folder.
2. Paste your sales and marketing data into the template. Alternatively, you can use the included `test_1` file filled with synthetic data to test the dashboard immediately.
3. Open the `.pbip` project in Power BI Desktop.
4. Update the `FolderPath` parameter to point to the folder where you saved the template.
5. Refresh and explore the dashboard!
