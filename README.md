<h1 align= "center">Retail Order Analysis</h1>
# Global Mart Sales Analysis (2022-2023)

## Project Overview
This project analyzes the retail orders of the Global Mart sales dataset for the years 2022 and 2023. The analysis was conducted using Python (Jupyter Notebook) for data processing and SQL (MySQL) for querying. The project includes data cleaning, processing, and answering five business-related questions.

## Dataset
The dataset was downloaded from Kaggle using the API and includes sales data for Global Mart from 2022 to 2023. It contains information about orders, products, categories, regions, and revenue.

## Project Steps

### 1. Downloading Dataset
- The dataset was downloaded using Kaggle's API. 
- The file was unzipped, and data was loaded using Pandas.

### 2. Data Processing and Cleaning (Pandas)
- Handled null values.
- Renamed columns for consistency (lowercase and replacing spaces with underscores).
- Derived new columns: `discount`, `sale_price`, and `profit`.
- Converted `order_date` to datetime format.
- Unnecessary columns (`cost_price`, `list_price`, `discount_percent`) were dropped.
- The cleaned data was then loaded into a MySQL database (`df_orders`).

### 3. Loading Data to MySQL
- The data was stored in a MySQL database to perform SQL queries.

### 4. SQL Ad-hoc Queries
1. **Top 10 highest revenue-generating products.**
2. **Top 5 highest selling products in each region.**
3. **Month-over-month growth comparison for 2022 and 2023 sales.**
4. **Month with the highest sales for each category.**
5. **Sub-category with the highest profit growth in 2023 compared to 2022.**

## Technologies Used
- **Python**: Data processing and analysis (Pandas, NumPy)
- **Jupyter Notebook**: Interactive coding
- **SQL**: Querying and analysis (MySQL)
- **Kaggle API**: Dataset download

## How to Use This Project

### 1. Prerequisites
Install the required Python libraries using the `requirements.txt` file:
```bash
pip install -r requirements.txt
