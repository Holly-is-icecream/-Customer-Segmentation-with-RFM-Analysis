
# 🛍️ Online Retail Data Analytics Portfolio Project

## 📌 Project Overview
This project analyzes the "Online Retail" dataset from the UCI Machine Learning Repository. It includes data cleaning, sales analysis, customer segmentation using the RFM model, and country-level revenue comparisons. It also features a dashboard visualization built with Tableau (or Power BI).

---

## 🗂 Dataset Details

- **Source**: UCI Online Retail Dataset ([link](https://archive.ics.uci.edu/ml/datasets/online+retail))
- **Data Format**: Excel
- **Features**:
  - Transactional data: `InvoiceNo`, `StockCode`, `Description`, `Quantity`, `InvoiceDate`, `UnitPrice`, `CustomerID`, `Country`
  - Time range: December 2010 – December 2011

---

## 🔧 Tools & Libraries

- Python (pandas, matplotlib, seaborn)
- Jupyter Notebook
- Tableau / Power BI
- Excel

---

## 📊 Key Analyses

### ✅ 1. Data Cleaning
- Removed rows with missing `CustomerID`
- Filtered out cancelled transactions (InvoiceNo starts with "C")
- Created `TotalPrice = Quantity × UnitPrice`
- Converted `InvoiceDate` to datetime and extracted `Date`

---

### 📈 2. Daily Sales Trend
- Aggregated sales by day and plotted trend line

### 🏷 3. Top 10 Most Sold Products
- Visualized using horizontal bar chart

### 🌍 4. Country-Level Revenue Comparison
- Summarized and ranked countries by total revenue
- Visualized the top 10 countries using bar charts

### 📊 5. Customer Segmentation (RFM Analysis)
- Calculated Recency, Frequency, and Monetary values for each customer
- Scored each metric and built a composite RFM score
- Classified customers as: `Top Customer`, `Loyal`, `Frequent`, `Recent`, `Others`
- Visualized customer segment distribution

### 📊 6. Interactive Dashboard
- A Tableau/Power BI dashboard was built to display:
  - Sales trends
  - Product performance
  - Country-level KPIs
  - Customer segments

---

## 📂 Project Structure

```
online-retail-analysis/
├── data/
│   └── Online Retail.xlsx
├── notebooks/
│   ├── sales_trends.ipynb
│   ├── top_products.ipynb
│   ├── country_revenue.ipynb
│   └── rfm_analysis.ipynb
├── dashboard/
│   └── retail_dashboard.twb (or .pbix)
├── images/
│   ├── sales_trend.png
│   ├── top_products.png
│   └── country_revenue.png
├── README.md
```

---

## 📌 Key Insights

- 🇬🇧 UK dominates sales, but there are high-value international customers
- 📦 A few products generate disproportionately high revenue
- 🧍‍♂️ Customers with high frequency + recent purchase behavior form the core revenue base

---

## 🧠 Future Improvements

- Predictive modeling for churn or purchase likelihood
- NLP on product descriptions to cluster categories
- Live connection with databases or data warehouses

---

## 👤 Author

陈浩林  
📧 Email: [your-email@example.com]  
🌐 GitHub: [https://github.com/your-username]  
📊 Tableau Public: [your-tableau-profile-link] (if available)
