# Elevate-Labs-task-6
# 🛒 Sales Trend Analysis Using MySQL

This project performs **monthly sales trend analysis** on e-commerce order data using SQL in **MySQL Workbench**. It calculates **monthly revenue** and **order volume** from a cleaned sales dataset.

---

## 📁 Dataset

We used a cleaned CSV file based on a Kaggle dataset. The file has the following structure:


> 💡 `amount` = total value of an order (already calculated).  
> `order_date` is in `YYYY-MM-DD` format.

---

## ⚙️ Requirements

- MySQL Workbench
- A local MySQL Server
- Cleaned CSV file (e.g., `online_sales_dataset.csv`)

---

## 🚀 Setup Instructions

### 1. Create Database and Table

Open MySQL Workbench and run:

```sql
CREATE DATABASE IF NOT EXISTS sales_db;
USE sales_db;

CREATE TABLE online_sales (
    order_id INT,
    product_id INT,
    order_date DATE,
    amount DECIMAL(10, 2)
);
