# Superstore Sales – Power BI Analysis

## Objective
The objective of this project is to transform raw sales data into meaningful insights through interactive Power BI dashboards.  
The analysis tracks overall business performance, identifies high-value customers and products, and highlights key trends to support data-driven decision-making.

---

## Project Structure
```text
Superstore_Sales_Analysis/
├── Data/ # Raw data before any cleaning
├── Coding_and_Data_Modeling/ # Jupyter Notebook for ETL, Data Modeling, DWH, and processed tables(Dim, Fact)
├── PowerBI/ # Power BI Desktop file with interactive dashboards
└── README.md # Project overview and instructions
```

---

## Data

- **Folder:** `Data/`  
- **Contents:** `superstore.csv` – Main dataset with details about orders, products, customers, regions, and shipping modes.  
- **Source:** [Superstore Dataset – Final (Kaggle)](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)

**Notes:**
- Data is kept raw; cleaning and transformation are performed in the notebook.
- Ensure the dataset exists in the `Data/` folder before running the notebook.

---

## Coding and Data Modeling

- **Folder:** `Coding_and_Data_Modeling/`  
- **Notebook:** `Superstore_Data_Analysis.ipynb`  
- **Processed Tables:**  
  - Dimension Tables: `Dim_Customer.csv`, `Dim_Product.csv`, `Dim_Geography.csv`, `Dim_Ship.csv`, `Dim_Date.csv`  
  - Fact Table: `Fact_Sales.csv`  

### Notebook Overview

1. **Loading and Reading Data**
   - Import the raw dataset from `Data/` and explore initial structure.

2. **Transformation and Preprocessing**
   - 2.1 **Info and Describe:** Check data types, nulls, and summary statistics.  
   - 2.2 **Data Cleaning:** Handle missing values, correct data types, and remove inconsistencies.

3. **Feature Engineering**
   - Create new features for analysis and reporting.

4. **Star Schema Transformation**
   - Split dataset into a **fact table** (`Fact_Sales`) and **dimension tables** (`Dim_*`).

5. **Saving Fact and Dimension Tables**
   - Export processed tables as CSV files for use in Power BI dashboards.

---

## Power BI

- **Folder:** `PowerBI/`  
- **File:** `Superstore_Sales.pbix`  

### Dashboard Overview

1. **Executive Summary:** Main KPIs and yearly sales trends.  
2. **Customer Analysis:** Top customers, sales by segment, and geographic distribution.  
3. **Product Performance:** Top products by sales and profit, sales by shipping mode, and product category performance.

**Notes:**
- Dashboards use processed tables from the notebook.
- Open `.pbix` in **Power BI Desktop** to view interactive dashboards.

---

## How to Use

1. Download the dataset from Kaggle and place it in the `Data/` folder.  
2. Run `Superstore_Data_Analysis.ipynb` to clean, transform, and create fact/dimension tables (if needed).  
3. Use the CSV files in `Coding_and_Data_Modeling/` for Power BI or analysis.  
4. Open `Superstore_Sales.pbix` in Power BI Desktop to explore dashboards.

---

## Outcome

A fully processed **data warehouse** with fact and dimension tables, and an interactive **Power BI dashboard** that allows tracking sales performance, analyzing customer behavior, and making data-driven business decisions.
