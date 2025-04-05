
# 🍕 Pizza Sales Analysis using SQL

Welcome to the **Pizza Sales Analysis** project! This repository contains a full SQL-based analysis of pizza sales data, focusing on business insights such as revenue, order trends, popular items, and customer behavior.

---

## 📊 Project Overview

This project explores a fictional pizza restaurant's sales data to uncover insights and trends using SQL. The goal is to help business stakeholders make informed decisions regarding menu offerings, staffing, inventory, and marketing.

---

## 🛠️ Tools & Technologies

- **SQL** (Structured Query Language)
- **MySQL / PostgreSQL / SQL Server** (whichever you're using)
- **DB Management Tool**: (e.g. MySQL Workbench, DBeaver, pgAdmin)
- **Data Source**: Pizza sales dataset (CSV/Excel imported into SQL database)

---

## 📁 Repository Structure

```
📦 pizza-sales-analysis/
├── 📄 schema.sql           # SQL to create tables and insert data
├── 📄 pizza_queries.sql    # All the analysis queries
├── 📄 ERD.png              # Entity Relationship Diagram
├── 📊 dashboards/          # (Optional) Visualization dashboards (Power BI, Tableau, etc.)
└── 📘 README.md            # Project documentation
```

---

## 🔍 Key Insights & Questions Answered

- ✅ Total revenue, orders, and average order value
- 🍕 Best-selling pizzas by quantity and revenue
- 🕒 Peak order times (by day of the week & hour)
- 🧾 Order distribution by size and category
- 📉 Underperforming pizzas and potential optimization areas

---

## 📈 Sample Queries

```sql
-- Total Revenue
SELECT ROUND(SUM(total_price), 2) AS total_revenue
FROM pizza_sales;

-- Best Selling Pizzas
SELECT pizza_name, SUM(quantity) AS total_sold
FROM pizza_sales
GROUP BY pizza_name
ORDER BY total_sold DESC
LIMIT 5;
```

---

## 📌 Getting Started

1. Clone this repository
2. Import the `schema.sql` file into your SQL environment
3. Load the dataset if not already included
4. Run queries from `pizza_queries.sql` for analysis

---

## 📚 Dataset Source

Fictional pizza sales dataset (custom-made or sourced from [Kaggle](https://www.kaggle.com) or another platform). Make sure to give credit if you're using someone else's dataset.

---

## 🤝 Contributing

Feel free to open issues or submit PRs if you want to improve or add new insights to the analysis!

---

## 📜 License

MIT License

---

