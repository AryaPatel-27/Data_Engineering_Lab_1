# E-Commerce Data Engineering Lab

This project implements a 12-step Data Engineering workflow using an e-commerce transaction dataset.
The notebook loads, profiles, cleans, transforms, and analyzes the transaction data.
A secondary city metadata dataset is used to enrich the transaction records.
The project includes feature engineering, city-level aggregation, and data serialization.
The final enriched dataset is saved in both CSV and JSON formats.

## Project Structure

```text
ecommerce-data-engineering-lab/
│
├── data/
│   ├── ecommerce_500.csv
│   └── metadata.csv
│
├── notebook/
│   └── ecommerce_data_engineering.ipynb
│
├── output/
│   ├── enriched_ecommerce.csv
│   └── enriched_ecommerce.json
│
├── .gitignore
├── README.md
└── requirements.txt
```

## Requirements

* Python 3.x
* Pandas
* NumPy
* Jupyter Notebook

## Quick Start

### 1. Clone the repository

```bash
git clone https://github.com/AryaPatel-27/Data_Engineering_Lab_1.git
```

### 2. Create a virtual environment

```bash
python -m venv venv
```

### 3. Activate the virtual environment

**Windows PowerShell:**

```powershell
.\venv\Scripts\Activate.ps1
```

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

### 5. Start Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
notebook/ecommerce_data_engineering.ipynb
```

Run the notebook from top to bottom.

## Data Sources

### Primary Dataset

`ecommerce_500.csv` contains the e-commerce transaction data used for the main analysis. It includes fields such as date, customer ID, product, price, quantity, coupon code, and shipping city.

**Source:** https://github.com/AryaPatel-27/Data_Engineering_Lab_1/blob/main/data/ecommerce_500.csv

### Secondary Dataset

`metadata.csv` contains city-level metadata used to enrich the transaction data. It includes information such as province, country, timezone, population, latitude, and longitude.

**Source:** https://github.com/AryaPatel-27/Data_Engineering_Lab_1/blob/main/data/metadata.csv

## Data Engineering Workflow

The notebook follows the required 12-step workflow:

1. Hello, Data!
2. Pick the Right Container
3. Implement Functions and Data Structure
4. Bulk Loaded
5. Quick Profiling
6. Spot the Grime
7. Cleaning Rules
8. Transformations
9. Feature Engineering
10. Mini-Aggregation
11. Serialization Checkpoint
12. Soft Interview Reflection

## Main Features

* Loads transaction and metadata CSV files
* Uses Python dictionaries and sets
* Implements Python classes and methods
* Profiles prices and shipping cities
* Checks data quality
* Cleans and standardizes transaction data
* Extracts discount percentages from coupon codes
* Calculates discounted price and revenue
* Creates `days_since_purchase` and `gross_value`
* Joins transaction data with city metadata
* Calculates revenue and customer statistics by city
* Exports enriched data to CSV and JSON

## Output

The processed data is saved in the `output/` folder:

```text
enriched_ecommerce.csv
enriched_ecommerce.json
```

These files contain the cleaned, transformed, and enriched transaction data.


