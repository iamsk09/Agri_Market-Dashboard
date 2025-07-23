## 📊 Project Title:  
**AgriMarket Insights Dashboard**

---

## 📝 Project Description:

Developed a Power BI dashboard to analyze sales and customer activity at a Farmers Market. The dataset included vendors, booths, products, and transactions. This interactive solution provides real-time insights for vendors and organizers to monitor sales, track customer behavior, and optimize product and booth management.

---
## 🔍 Approach and Process

### 1️⃣ Data Cleaning
• Cleaned and structured raw CSV files containing customer, vendor, and transaction data  
• Standardized column names, handled missing values, and removed duplicates  
• Converted price, quantity, and date fields to appropriate data types  

### 2️⃣ Data Modeling
• **Fact Table**: Transaction-level sales data  
• **Dimension Tables**:  
  - **Customer Table** – contains customer ID, name, and location info  
  - **Vendor Table** – vendor and booth relationships  
  - **Product Table** – category and product pricing info  
• All tables linked via primary-foreign keys like `customer_id`, `vendor_id`, and `product_id`  

### 3️⃣ DAX Measures
• `Total_Sales = SUMX(quantity × cost_to_customer_per_qty)`  
• `Total Quantity = SUM(quantity)`  
• `Unique Customers = DISTINCTCOUNT(customer_id)`  
• `Customer_FULL_Name = [customer_first_name] & "_" & [customer_last_name]`  

### 4️⃣ Power BI Visualizations
• **Slicers** – Allow filtering by Product, Customer, Vendor, and Date  
• **KPI Cards** – Display total quantity sold, total sales, unique customers, total booths/vendors  
• **Pie & Donut Charts** – Top-selling products and vendor contributions  
• **Bar Charts & Tables** – Top customers by sales and quantity  
• **Zip Code Analysis** – Sales and quantity distribution by customer location  
• **Word Cloud** – Visual emphasis on high-value customers based on purchase volume  

---

## 📈 Key Insights:

✅ 3 products account for **90%+ of sales** → demand is highly concentrated  
✅ 30% of customers drive **over 50% of purchases** → strong case for loyalty programs  
✅ Uneven vendor performance → opportunities for **inventory/booth reallocation**  
✅ Only 29 unique buyers out of 1003 total purchases → **repeat buyers dominate**, potential for outreach  

---

## ⚒️ Tools & Techniques Used:

✅ Microsoft Power BI Desktop for modeling, DAX measures, and interactive visuals  
✅ Excel (.CSV) for data storage and cleaning  
✅ Relationships created between tables using primary/foreign keys (e.g., `customer_id`, `vendor_id`)  
✅ DAX Measures for Total Sales, Quantity, and KPIs  

---

## 💡 Use Case / Practical Application:

✅ Market organizers to manage booths and track performance  
✅ Vendors to see which products and customers are most valuable  
✅ Data analysts to derive actionable business strategies based on patterns and metrics  


