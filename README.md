

---

# 📊 Sales_Analytics: Database Schema, Sample Data & Query Examples

## 1. Overview
This project creates a **Sales Analytics Database** to manage customers, products, salespersons, and orders.  
It includes **sample data inserts** and a wide range of **SQL queries** demonstrating filtering, grouping, ordering, aggregation, and advanced window functions.

---

## 2. Database Schema

### **Customers Table**
- Stores customer details.  
- **Columns:** `CustomerID`, `CustomerName`, `Gender`, `City`, `Email`  
- **Sample Data:** 30 customers across multiple cities.

### **Products Table**
- Stores product details.  
- **Columns:** `ProductID`, `ProductName`, `Category`, `Price`  
- **Sample Data:** Electronics & Furniture items.

### **Salespersons Table**
- Stores salesperson details.  
- **Columns:** `SalespersonID`, `SalespersonName`, `Region`, `TargetAmount`

### **Orders Table**
- Stores order transactions.  
- **Columns:** `OrderID`, `CustomerID`, `SalespersonID`, `ProductID`, `Quantity`, `OrderDate`  
- **Relationships:**  
  - `CustomerID` → Customers  
  - `SalespersonID` → Salespersons  
  - `ProductID` → Products  

---

## 3. Sample Queries

### **Basic Retrieval**
- Distinct cities from Customers  
- Distinct product categories  
- Customer names & emails (renamed as `Customer_Name`, `Email_ID`)  
- Products with tax, double price, or price filters  

### **Filtering**
- Customers from Hyderabad  
- Products priced above 10,000  
- Orders placed after `2025-01-12`  
- Female customers in Chennai  
- Products not in Electronics/Furniture  

### **Ordering & Limiting**
- Customers ordered by name  
- Top 3 products by price  
- Top 3 expensive products > 5000  
- Customers in Chennai/Pune/Hyderabad sorted by name  

### **Aggregation & Grouping**
- Number of customers in each city  
- Number of customers by gender  
- Cities with customer count > 2  
- Customers with more than 3 orders  
- Average price per category (only > 5000)  

### **Window Functions**
- Earliest & latest order dates  
- Total orders per customer using `COUNT OVER`  
- Product price ranking using `RANK()`  
- Ranking within each category using `PARTITION BY`  

---

## 4. Key Highlights
- Demonstrates **SQL fundamentals**: `SELECT`, `WHERE`, `ORDER BY`, `GROUP BY`, `HAVING`.  
- Uses **aggregate functions**: `COUNT`, `AVG`, `MIN`, `MAX`.  
- Applies **window functions**: `RANK()`, `COUNT() OVER`.  
- Provides **realistic sample data** for analytics scenarios.  

---

✅ This README makes your project **professional and portfolio-ready**.  
Would you like me to also create a **visual ER diagram (Entity-Relationship)** for this schema so you can include it in your documentation?
