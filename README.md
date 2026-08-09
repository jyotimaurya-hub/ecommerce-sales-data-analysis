# 🛒 E-commerce Sales Data Analysis

A Python-based exploratory data analysis project focused on analyzing e-commerce sales data using Pandas, NumPy, Seaborn, and Matplotlib.

## 📌 Project Overview

This project analyzes an e-commerce sales dataset containing 5,000 transactions and 12 columns.

The analysis covers data inspection, missing-value checking, date transformation, region encoding, categorical and numerical analysis, and data visualization.

## 🎯 Objectives

- Understand the structure of the e-commerce dataset
- Check data types and statistical information
- Check for missing values
- Convert order dates into datetime format
- Extract day, month, and year from order dates
- Convert region categories into numerical values
- Separate categorical and numerical columns
- Analyze numerical distributions and skewness
- Identify potential outliers
- Study relationships between variables and revenue
- Analyze revenue across product categories and payment methods
- Analyze average discount across categories

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Seaborn
- Matplotlib
- Jupyter Notebook

## 📂 Dataset

**Dataset:** `ecommerce_sales_analytics_5000.csv`

The dataset contains **5,000 records and 12 columns**.

### Columns

| Column | Description |
|---|---|
| order_id | Unique order identifier |
| order_date | Date of the order |
| customer_id | Customer identifier |
| product_category | Category of the purchased product |
| region | Customer/order region |
| quantity | Quantity purchased |
| unit_price | Price per unit |
| discount | Discount applied |
| payment_method | Payment method used |
| delivery_days | Number of days taken for delivery |
| customer_rating | Customer rating |
| revenue | Revenue generated from the order |

## 🔍 Data Analysis Process

### 1. Data Inspection

The project uses Pandas functions such as:

- `head()`
- `tail()`
- `shape`
- `info()`
- `describe()`
- `columns`
- `index`

The dataset contains **5,000 rows and 12 columns**.

### 2. Missing Value Check

Missing values were checked using:

```python
df.isnull().sum()
```

The dataset contains **no missing values**.

### 3. Date Transformation

The `order_date` column was converted into datetime format.

Three additional features were created:

- `order__day`
- `order__month`
- `order_year`

The original `order_date` column was then removed.

### 4. Region Transformation

The `region` column was converted into numerical values:

| Region | Code |
|---|---:|
| West | 0 |
| East | 1 |
| North | 2 |
| South | 3 |

### 5. Categorical and Numerical Variables

**Categorical variables**
- `product_category`
- `payment_method`

**Numerical variables**
- `order_id`
- `customer_id`
- `region`
- `quantity`
- `unit_price`
- `discount`
- `delivery_days`
- `customer_rating`
- `revenue`
- `order__day`
- `order__month`
- `order_year`

## 📊 Exploratory Data Analysis

The project performs analysis on:

- Product categories
- Payment methods
- Revenue
- Unit price
- Quantity
- Discount
- Delivery days
- Customer ratings
- Order dates
- Regions

## 📈 Data Visualizations

The notebook includes:

- Distribution plots for numerical variables
- Box plots for numerical variables
- Count plots for categorical variables
- Scatter plots between numerical variables and revenue
- Scatter plots between numerical variables and unit price
- Bar plots showing revenue by categorical variables
- Bar plots showing average discount by category

These visualizations help understand distributions, relationships, outliers, revenue patterns, and discount patterns in the dataset.

## 📌 Statistical Analysis

The project calculates skewness for numerical variables to understand data distributions.

Descriptive statistics are calculated using:

```python
df.describe().T
```

## 💡 Key Analysis Areas

This project helps explore:

- Product category performance
- Revenue patterns
- Customer behavior
- Payment method distribution
- Regional information
- Pricing patterns
- Discount patterns
- Delivery performance
- Customer ratings
- Relationships between numerical variables

## 📁 Project Structure

```text
ecommerce-sales-data-analysis/
│
├── ecommerce_sales_analytics_5000.ipynb
├── ecommerce_sales_analytics_5000.csv
└── README.md
```

## 🚀 How to Run the Project

### 1. Clone the repository

```bash
git clone <your-repository-url>
```

### 2. Open the project

Open the project folder in **VS Code** or **Jupyter Notebook**.

### 3. Install required libraries

```bash
pip install pandas numpy seaborn matplotlib
```

### 4. Run the notebook

Open:

```text
ecommerce_sales_analytics_5000.ipynb
```

Run the notebook cells from top to bottom.

## 👩‍💻 Skills Demonstrated

- Python
- Pandas
- NumPy
- Data Inspection
- Data Cleaning
- Date-Time Processing
- Feature Transformation
- Exploratory Data Analysis
- Statistical Analysis
- Data Visualization
- Seaborn
- Matplotlib

## 📌 Conclusion

This project demonstrates an end-to-end exploratory data analysis workflow using Python and Pandas.

It covers data inspection, missing-value checking, date transformation, categorical and numerical analysis, statistical analysis, and visualization to understand e-commerce sales data.

