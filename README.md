# ApexPlanet Data Analytics Internship — Sales Data Cleaning

## Project Overview

This project focuses on exploring, cleaning, validating, and transforming a sales dataset using Python and pandas. It was completed as part of the ApexPlanet Data Analytics internship task.

## Dataset

The original dataset contains 1,000 sales records and 12 columns, including order details, customer information, product categories, quantities, unit prices, and sales totals.

## Tools Used

- Python
- pandas
- NumPy
- Jupyter Notebook in Visual Studio Code
- openpyxl
- Git and GitHub

## Work Completed

1. Inspected dataset dimensions, column types, descriptive statistics, and unique values.
2. Assessed missing values and duplicate records.
3. Filled missing ages using the median and missing cities with `Unknown`.
4. Converted order dates to datetime format.
5. Investigated repeated order IDs and assigned unique identifiers while preserving original IDs in `Original_Order_ID`.
6. Validated sales totals against quantity multiplied by unit price.
7. Created additional time-based and age-group columns.
8. Exported the cleaned data to CSV and Excel formats.

## Validation Results

- Final rows: 1,000
- Final columns: 16
- Missing values: 0
- Exact duplicate rows: 0
- Duplicate order IDs: 0
- Sales calculation mismatches: 0

## Important Note

Repeated order IDs were disambiguated under the assumption that each row requires a unique identifier. The original IDs were preserved for traceability. These assigned IDs should be confirmed against the source system before being treated as authoritative order corrections.

## Project Files

- `ApexPlanet_Data_Cleaning.ipynb` — notebook containing exploration, cleaning, and validation steps
- `cleaned_sales_dataset.csv` — cleaned dataset in CSV format
- `cleaned_sales_dataset.xlsx` — cleaned dataset in Excel format
- `data_quality_report.csv` — summary of data quality findings and actions

## How to Run

1. Install Python and Visual Studio Code with the Jupyter extension.
2. Install dependencies using `pip install pandas numpy openpyxl`.
3. Place the original Excel dataset in the project folder.
4. Open and run `ApexPlanet_Data_Cleaning.ipynb` from top to bottom.

## Conclusion

The cleaning and validation process addressed missing values, date formatting, repeated order identifiers, and sales calculation checks. The resulting dataset is ready for further exploratory data analysis, subject to verification of the assumed order ID corrections.
