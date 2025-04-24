
# 📦 Online Retail Data Analysis (UCI Dataset)

## 📌 Project Overview
This project analyzes the "Online Retail" dataset from the UCI Machine Learning Repository. It focuses on data cleaning, trend analysis, and product popularity to demonstrate core data analytics skills using Python.

---

## 📁 Dataset Information

- **Source**: UCI Machine Learning Repository - [Online Retail Data](https://archive.ics.uci.edu/ml/datasets/online+retail)
- **Format**: Excel (.xlsx)
- **Description**: Transactional data from a UK-based online retailer, from 2010-2011.

### Key Columns:
- `InvoiceNo`, `StockCode`, `Description`, `Quantity`, `InvoiceDate`, `UnitPrice`, `CustomerID`, `Country`

---

## 🔧 Tools & Libraries

- Python 3.x
- pandas
- matplotlib
- Jupyter Notebook

---

## 🧹 Data Cleaning Steps

1. Removed rows with missing `CustomerID`
2. Filtered out canceled orders (InvoiceNo starts with "C")
3. Created a new column `TotalPrice = Quantity * UnitPrice`
4. Converted `InvoiceDate` to datetime format and extracted `Date` column

---

## 📊 Exploratory Analysis

### 1. 📈 Daily Sales Trend

A time series plot was created to visualize total sales per day.

```python
daily_sales = df.groupby("Date")["TotalPrice"].sum()
daily_sales.plot()
```

### 2. 🏷 Top 10 Most Sold Products

A horizontal bar chart showing the top-selling products by total quantity.

```python
top_products = df.groupby("Description")["Quantity"].sum().sort_values(ascending=False).head(10)
```

---

## 📂 Project Structure

```
online-retail-analysis/
├── data/
│   └── Online Retail.xlsx
├── notebooks/
│   └── analysis.ipynb
├── images/
│   └── sales_trend.png
├── README.md
```

---

## 🚀 Next Steps

- Add country-level revenue comparison
- Implement RFM (Recency, Frequency, Monetary) customer segmentation
- Build an interactive dashboard with Tableau or Power BI

---

## 👤 Author

陈浩林  
GitHub: [your-github-link]  
Email: [your-email-address]
