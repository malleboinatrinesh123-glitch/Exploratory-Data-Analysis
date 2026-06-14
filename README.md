# ☕ Dirty Cafe Sales Analysis

## 📌 Project Overview
This project performs Exploratory Data Analysis (EDA) and Business Intelligence on the Dirty Cafe Sales Dataset. The goal is to uncover trends, customer behavior, product performance, and sales insights using Python, SQL, and data visualization techniques.

## 🎯 Objectives
- Clean and preprocess raw cafe sales data.
- Perform descriptive statistical analysis.
- Identify sales trends and customer purchasing patterns.
- Answer business questions using SQL queries.
- Create visualizations and dashboard-ready insights.

---

## 📂 Dataset
The dataset contains cafe transaction records including:
- Transaction Date
- Customer ID
- Item Purchased
- Quantity
- Price Per Unit
- Total Spent
- Payment Method

---

## 🛠️ Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SQLite / SQL
- Google Colab

---

## 📊 Exploratory Data Analysis

### Data Cleaning
- Removed duplicate records
- Handled missing values
- Corrected data types
- Checked data consistency

### Descriptive Statistics
- Mean, Median, Mode
- Standard Deviation
- Distribution Analysis

### Visualizations
- Histograms
- Bar Charts
- Correlation Heatmaps
- Pair Plots
- Monthly Revenue Trends

---

## 📈 Business Questions

### 1. Top Selling Products
Identify products generating the highest revenue.

### 2. Revenue by Payment Method
Analyze customer payment preferences.

### 3. Monthly Sales Trends
Track revenue growth over time.

### 4. Customer Purchase Patterns
Identify repeat customers and spending habits.

### 5. Average Order Value
Measure customer transaction value.

---

## 🗄️ Sample SQL Queries

### Top 5 Products by Revenue

```sql
SELECT Item,
       SUM([Total Spent]) AS Revenue
FROM cafe_sales
GROUP BY Item
ORDER BY Revenue DESC
LIMIT 5;
```

### Revenue by Payment Method

```sql
SELECT [Payment Method],
       SUM([Total Spent]) AS Revenue
FROM cafe_sales
GROUP BY [Payment Method];
```

### Monthly Sales Trend

```sql
SELECT DATE_TRUNC('month', [Transaction Date]) AS Month,
       SUM([Total Spent]) AS Revenue
FROM cafe_sales
GROUP BY Month
ORDER BY Month;
```

---

## 📷 Project Outputs
- Cleaned Dataset
- EDA Report
- SQL Query Results
- Visualizations
- Business Insights Dashboard

---

## 🚀 How to Run

1. Clone the repository:

```bash
git clone https://github.com/your-username/dirty-cafe-sales-analysis.git
```

2. Install required libraries:

```bash
pip install pandas numpy matplotlib seaborn
```

3. Open the notebook in Google Colab or Jupyter Notebook.

4. Upload the dataset and run all cells.

---

