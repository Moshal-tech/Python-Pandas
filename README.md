# Python-Pandas

# 🐍 Python Pandas | Retail & Sales Data Analysis

### 🟢 Data Technician Bootcamp | Week 6 – Python Data Analysis & Visualisation

![Python](https://img.shields.io/badge/Python-Programming-3776AB)
![Pandas](https://img.shields.io/badge/Pandas-Data_Analysis-150458)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Data_Visualisation-orange)
![Google Colab](https://img.shields.io/badge/Google-Colab-F9AB00)
![Data Cleaning](https://img.shields.io/badge/Data-Cleaning-brightgreen)
![Status](https://img.shields.io/badge/Project-Bootcamp_Training-success)

---

## 🌟 Project Overview

This project was completed as part of my **Data Technician Bootcamp**, focusing on using **Python, Pandas and Matplotlib** to explore, clean, manipulate and visualise datasets.

Working in **Google Colab and Jupyter Notebooks**, I developed practical data analysis skills through exercises involving DataFrames, data selection, filtering, missing-value handling and statistical analysis.

The project strengthened my understanding of how Python can be used to transform raw data into meaningful insights, with techniques applicable to **retail sales performance, product analysis, customer trends and business reporting**.

---

## 🛠️ Tools & Technologies

| Technology | Purpose |
|---|---|
| 🐍 Python | Data analysis and programming |
| 🐼 Pandas | Data cleaning, manipulation and analysis |
| 📊 Matplotlib | Creating charts and visualisations |
| 🟠 Google Colab | Writing and executing Python notebooks |
| 📓 Jupyter Notebook | Documenting data analysis workflows |
| 📂 CSV Files | Importing and analysing structured datasets |

---

## 🚀 Key Skills Demonstrated

### 🔍 1. Data Exploration & Inspection

Used Pandas to load, inspect and understand datasets.

- `pd.read_csv()` – Import CSV datasets.
- `.head()` and `.tail()` – Preview data records.
- `.info()` – Examine data types and missing values.
- `.describe()` – Generate descriptive statistics.
- `.shape` – Identify the number of rows and columns.
- `.value_counts()` – Examine the frequency of values.

These techniques support the initial assessment of dataset quality, structure and suitability for analysis.

### 🎯 2. Data Filtering & Slicing

Applied Pandas indexing techniques to retrieve relevant information.

- `.loc[]` – Select rows and columns using labels or conditions.
- `.iloc[]` – Select data using integer positions.
- Boolean filtering – Extract records meeting specific criteria.
- Column selection – Focus on relevant analytical variables.
- Conditional expressions – Identify subsets of business data.

**Retail application:** Filtering high-value transactions, selecting particular products and analysing sales in specific regions.

### 🧹 3. Data Cleaning & Missing-Value Handling

Explored techniques for improving dataset quality.

- `.isnull()` and `.isna()` – Identify missing values.
- `.dropna()` – Remove incomplete records where appropriate.
- `.fillna()` – Replace missing values using suitable methods.
- `.drop_duplicates()` – Identify and remove duplicate records.
- `.astype()` – Convert columns into appropriate data types.
- `.rename()` – Improve column names and readability.

These techniques help prepare data for reliable calculations, analysis and reporting.

### 🔄 4. Data Manipulation & Transformation

Used Pandas methods to reorganise and summarise datasets.

- `.groupby()` – Aggregate records by category.
- `.sort_values()` – Rank data in ascending or descending order.
- `.agg()` – Calculate multiple summary statistics.
- `.mean()`, `.sum()`, `.min()` and `.max()` – Analyse numerical values.
- Created calculated columns to support additional analysis.

**Retail application:** Comparing sales performance across product categories and identifying patterns in revenue and transaction volumes.

### 📊 5. Data Visualisation Using Matplotlib

Explored Python visualisation techniques for communicating data patterns.

| Visualisation | Analytical Purpose |
|---|---|
| 📊 Bar Chart | Compare sales by product category |
| 📈 Line Chart | Analyse sales trends over time |
| 🥧 Pie Chart | Show category contribution to total sales |
| 📉 Histogram | Examine distributions of numerical values |
| 🔵 Scatter Plot | Explore relationships between variables |

Used visualisations to make analytical findings easier to understand and communicate.

---

## 💻 Example Python Code – Retail Sales Analysis

The examples below demonstrate the analytical techniques using an illustrative `retail_sales.csv` dataset with columns including `Product`, `Category`, `Region` and `Sales`.

### 🟢 1. Import and Explore Data

```python
import pandas as pd
import matplotlib.pyplot as plt

df = pd.read_csv("retail_sales.csv")

print(df.head())
print(df.info())
print(df.describe())
```

### 🔵 2. Filter and Slice Data

```python
# Filter high-value sales
high_sales = df[df["Sales"] > 500]

# Select columns using loc
selected = df.loc[:, ["Product", "Category", "Sales"]]

# Select first 10 rows using iloc
first_ten = df.iloc[:10]

print(high_sales)
```

### 🟠 3. Handle Missing Values

```python
# Check missing values
print(df.isnull().sum())

# Remove rows with missing critical fields
df = df.dropna(subset=["Product", "Sales"])

# Fill missing region values
df["Region"] = df["Region"].fillna("Unknown")
```

### 🟣 4. Group and Sort Sales Data

```python
# Calculate total sales by category
category_sales = df.groupby("Category")["Sales"].sum()

# Sort categories by sales
category_sales = category_sales.sort_values(
    ascending=False
)

print(category_sales)
```

### 🟡 5. Visualise Sales by Category

```python
category_sales.plot(
    kind="bar",
    figsize=(10, 5),
    title="Total Sales by Product Category"
)

plt.xlabel("Product Category")
plt.ylabel("Total Sales")
plt.tight_layout()
plt.show()
```

---

## 🛍️ Retail & Sales Analytics Applications

The techniques developed can be used to:

- 💰 Analyse revenue and transaction values.
- 📦 Identify top-performing product categories.
- 🌍 Compare sales across geographical regions.
- 📈 Investigate sales trends and patterns.
- 🔍 Identify missing, inconsistent or duplicate records.
- 📊 Produce summary statistics for management reporting.
- 🎯 Support data-driven commercial decisions.

---

## 🎯 Project Outcomes

✅ Strengthened practical Python and Pandas skills.

✅ Explored structured datasets using DataFrames.

✅ Applied filtering and slicing using `.loc[]` and `.iloc[]`.

✅ Developed knowledge of missing-value identification and handling.

✅ Used grouping, aggregation and sorting to summarise datasets.

✅ Explored Python visualisations using Pandas and Matplotlib.

✅ Improved understanding of exploratory data analysis and data quality.

✅ Developed transferable skills for retail analytics and business intelligence.

---

## 💡 Key Learning & Business Value

This project strengthened my ability to use **Python and Pandas to prepare, investigate and analyse structured data**.

Through practical exercises, I developed an understanding of the data analysis lifecycle, from importing raw datasets and identifying data quality issues to transforming information and presenting findings visually.

These skills provide a foundation for **data automation, exploratory data analysis, operational reporting and business intelligence**, supporting progression into Data Analyst, BI Analyst and Reporting Analyst roles.

---

## 🏷️ Skills & Keywords

`Python` `Pandas` `Matplotlib` `Google Colab` `Jupyter Notebook` `DataFrames` `Data Cleaning` `Data Manipulation` `Data Filtering` `.loc[]` `.iloc[]` `.groupby()` `.sort_values()` `.dropna()` `.fillna()` `Exploratory Data Analysis` `Data Visualisation` `Retail Analytics` `Sales Analysis` `Business Intelligence`

---

⭐ **Python data analysis project developed through my Data Technician Bootcamp portfolio.**
