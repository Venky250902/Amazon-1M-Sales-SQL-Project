# 🍎 Apple Retail Sales SQL Project  
### Analyzing 1M+ Sales Records with Advanced SQL

![Apple Store](./Apple_Changsha_RetailTeamMembers_09012021_big.jpg.slideshow-xlarge_2x.jpg)

---

## 🚀 Project Overview  

This project is a **deep-dive SQL analytics case study** built on **1M+ rows of Apple retail sales data**.  

The goal is simple:  
👉 Turn raw transactional data into **meaningful business insights** using SQL  

But what makes this project powerful is the scale, structure, and real-world business problems it solves.

---

## 🧠 What This Project Demonstrates  

- Writing **complex SQL queries** across multiple tables  
- Performing **real-world business analysis**  
- Handling **large-scale datasets (1M+ rows)**  
- Using **window functions, joins, aggregations, and CTEs**  
- Applying **query optimization techniques (indexing, EXPLAIN ANALYZE)**  

---

## 🏗️ Data Model (ERD)

![ERD](./erd.png)

This project is built on a **relational data model** with 5 core tables:

- `stores` → Store-level information  
- `category` → Product categories  
- `products` → Product details  
- `sales` → Transaction-level data  
- `warranty` → Post-sale claim insights  

👉 Designed with **primary + foreign key relationships** for accurate joins and analysis  

---

## 📊 Key Business Questions Solved  

### 🔹 Exploratory Analysis
- Which stores drive the most sales?
- Which categories generate the highest revenue?
- What are the best-selling products?

### 🔹 Operational Insights
- Stores with **no warranty claims**
- **Best-selling days** per store  
- Sales spikes across months and years  

### 🔹 Advanced Analytics
- 📈 Year-over-year growth by store  
- ⚠️ Warranty claim risk % by country  
- 💰 Price vs warranty correlation  
- 📊 Running revenue trends over time  

---

## ⚙️ Schema Design  

The database schema was carefully designed to ensure:

- Data integrity using **foreign key constraints**
- Clean relational structure for efficient querying
- Scalability for large datasets  

```sql
CREATE TABLE sales (
    sale_id VARCHAR(15) PRIMARY KEY,
    sale_date DATE,
    store_id VARCHAR(10),
    product_id VARCHAR(10),
    quantity INT
);
