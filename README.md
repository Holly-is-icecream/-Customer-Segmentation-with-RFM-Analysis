
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

### 🔍 Insights & Recommendations (Based on RFM Analysis)
🌟 1. Most Customers Fall Under the “Other” Category
The majority of customers have:
- Low purchase frequency
- No recent activity
- Low total spending
✅ Recommendation:**  
Deploy remarketing campaigns, personalized product recommendations, or targeted discount strategies to re-engage this large segment of inactive or low-value customers.

🌟 2. "Loyal" and "Frequent" Customer Segments Are Substantial
These segments consist of customers who buy regularly or have been active recently, representing a valuable user base for retention.
✅ Recommendation:**  
Introduce loyalty programs, point systems, VIP benefits, or exclusive access to maintain their interest and reward their consistency.

 🌟 3. "Top Customers" Are Few but High Value
These are the most engaged, high-spending, and recent customers — critical to business profitability.
✅ Recommendation:**  
Provide personalized services such as dedicated account managers, priority support, and tailored offers to improve satisfaction and maximize lifetime value.


## 👤 Author

陈浩林  
📧 Email: chenholly24@gmail.com
🌐 GitHub: [https://github.com/Holly-is-icecream]  
