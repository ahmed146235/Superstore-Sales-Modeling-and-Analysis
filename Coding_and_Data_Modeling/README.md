# Coding and Data Modeling Folder

This folder contains the Jupyter Notebook `Superstore_Data_Analysis.ipynb` which performs the full ETL, Data Modeling, and preparation for the Data Warehouse.

## Notebook Overview

The notebook is organized into the following sections:

1. **Loading and Reading Data**
   - Import the raw dataset from the `../Data/` folder.
   - Initial exploration of the dataset to understand structure and content.

2. **Transformation and Preprocessing of Data**
   2.1 **Info and Describe**
   - Review data types, null values, and basic statistics.  
   2.2 **Data Cleaning**
   - Handle missing values, correct data types, and remove inconsistencies.

3. **Feature Engineering**
   - Create new columns or features necessary for analysis and reporting.

4. **Splitting the Dataset into Fact and Dimension Tables (Star Schema Transformation)**
   - Transform the cleaned dataset into a **fact table** (`Sales`) and multiple **dimension tables** (`Customer`, `Product`, `Geography`, `Ship`, `Date`).

5. **Saving All Files (Dimensions and Fact)**
   - Export the processed tables as separate CSV files or other formats for use in Power BI dashboards.

## Notes

- Make sure the `Data/` folder exists and contains the raw dataset before running the notebook.
- Star Schema diagrams and additional explanations can be found in the `../Docs/` folder.
- This notebook serves as the main preprocessing and modeling step before creating Power BI dashboards.

