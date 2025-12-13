AdventureWorks Data Analysis Project

This project focuses on performing **data analysis** on the AdventureWorks dataset using **SQL** and **Excel**.

---

## 📊 Project Overview
The goal of this project was to clean, analyze, and visualize business data to gain insights into sales performance, profitability, and product trends.

---

## ⚙️ Data Preprocessing (SQL)
Data preprocessing was done using **SQL Server**, where I:
- Checked for **null values** and replaced them appropriately.  
- Handled **duplicates** using SQL scripts.  
- Cleaned and standardized categorical values (e.g., replacing `NA` with `UNKNOWN`).  
- Verified data consistency across multiple tables (Products, Regions, Resellers, Salespersons, and Targets) using `Dynamic SQL`.

---

## 📈 Dashboard (Excel)
After cleaning the data, I built an interactive **Excel dashboard** that includes:
- **modeling** to connect related tables.
- **Measures** to calculate Profits and Target Achievement Percentage
- Key Performance Indicators (KPI Cards) 📌
    * **Purpose:** Provides an immediate snapshot of the business's overall health.
    * **Metrics:** Displays **Total Sales**, **Total Profit**, **Total Quantity Sold**, and **Average Order Value**.
      
- **Charts** visualizing:
  -  Sales vs. Total Cost Trend (Line Chart) 📉
    
        * **Analysis:** Tracks the movement of Revenue against Costs over time (Months).
          
        * **Insight:** Helps identify seasonal trends and periods where costs spiked disproportionately to sales, affecting profit margins.
          
  - Sales by Category & Subcategory🚲
    
        * **Analysis:** A comparative view of sales performance across main categories (e.g., Bikes, Accessories) and detailed subcategories.
    
        * **Insight:** Identifies the "Bikes" products driving the majority of revenue versus underperforming items , when The most     category sold is "Components".

    ![Dashboard 1](dashboard1.PNG)
    
  - Sales by Region 🌍

      * **Analysis:** Displays the geographical distribution of sales across different territories (e.g., USA, Europe, UK).
        
      * **Insight:** Pinpoints the highest-revenue locations, highlighting that specific regions (USA) outperform others, which helps in planning regional marketing strategies.
 
   - Sales vs. Cost by Business Type  🏢
     
      * **Analysis:** Compares the Total Sales Revenue against Total Product Cost for different reseller types (e.g., Warehouse, Value Added Reseller, Specialty Bike Shop).
        
      * **Insight:** Evaluates the profitability of each business partner model. It reveals that while **"Warehouses"** might contribute the highest revenue volume, other types like **"Specially Bike Shop"** might yield better profit margins due to lower operational costs relative to sales.
      
      
    ![Dashboard 2](dashboard2.PNG)

        
  
---

## 🧠 Key Insights
- Identified high-performing categories and products.  
- Discovered seasonal patterns in sales and cost.  
- Analyzed profitability trends and average sales over time.

---

## 🛠️ Tools Used
- **SQL Server** — for data preprocessing and cleaning.  
- **Microsoft Excel** — for dashboard creation and visualization.

---
---

## 💬 Author
**Botayla Amin**  
Data Analyst | Data Scientist

📧 botaylaamin@gmail.com  

