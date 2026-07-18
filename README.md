# E-commerce Business Intelligence Pipeline (Olist Dataset)

This repository features a production-ready, modular data engineering and business intelligence pipeline built in Python. Utilizing the Olist Brazilian E-commerce dataset, the project transitions raw transactional records into data-driven strategic insights focused on executive C-level decision-making.

## 🏗️ Architecture & Pipeline Overview

The project is structured into three sequential, decoupled layers to ensure scalability and maintainability:

1. **`01_data_download.ipynb` (Ingestion Layer):** Programmatically connects to the KaggleHub API, handles dataset retrieval, provisions local infrastructure (`/data/raw`), and generates an automated data ingestion integrity report mapping file metadata and sizes.
2. **`02_data_cleaning.ipynb` (Processing Layer):** Conducts a comprehensive data quality audit (tracking null records and duplicates across 6 relational tables). Performs strategic joins and exports two highly optimized data models into `/data/processed`: `customer_sales` and `product_sales`.
3. **`03_business_analysis.ipynb` (Analytics Layer):** Consumes processed data to answer key business questions using an Object-Oriented plotting framework (Matplotlib) alongside custom text-based enterprise KPI dashboards.

---

## 📈 Key Enterprise Metrics & Insights

### 💳 Financial & Volume Summary

```text
======================================
         ENTERPRISE MAIN KPIS         
======================================
Total Orders:                   99,441
Total Customers:                96,096
Total Revenue:       R$  16,008,872.12
Average Order Value: R$         160.99
======================================
```

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone [https://github.com/franklin-azevedo/olist-ecommerce-analytics.git](https://github.com/franklin-azevedo/olist-ecommerce-analytics.git)
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Execute the notebooks sequentially inside the `notebooks/` folder.