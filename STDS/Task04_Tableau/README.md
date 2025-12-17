# 🇧🇷 Olist E-Commerce Analysis Dashboard

## 📊 Dashboard 1: Sales Performance Overview
This dashboard provides a high-level view of the company's financial health and market presence across Brazil.

### 1. Key Performance Indicators (KPIs) 📌
* **Metrics:** Displays **Total Revenue**, **Total Orders**.
* **Insight:** Gives an immediate snapshot of the total sales volume (approx. 13M BRL) and the scale of operations over the analysis period.

### 2. Sales by State 🗺️
* **Visualization:** A filled map of Brazil showing revenue concentration by state (e.g., SP, RJ, MG).
* **Analysis:** Color intensity represents sales volume—darker states generate more revenue.
* **Insight:** **São Paulo (SP)** is the dominant market, contributing the majority of sales, while northern regions show lower penetration, suggesting potential growth opportunities or logistical challenges in those areas.

### 3. Monthly Sales Trend 📈
* **Visualization:** Tracks Total Revenue over time (2016-2018).
* **Analysis:** visualizes the growth trajectory and seasonal peaks.
* **Insight:** There is a clear upward trend in sales.

### 4. Sales by Payment Method  💳
* **Visualization:** Breaks down the total number of orders based on the payment type used (Credit Card, Boleto, Voucher, Debit Card).
* **Analysis:** Shows customer payment preferences.
* **Insight:** **Credit Cards** are overwhelmingly the most popular payment method (likely due to installment options), followed by **Boleto**, which remains a crucial option for unbanked customers in Brazil.

### 5.  Product Categories by Revenue 🏆
* **Visualization:** A horizontal bar chart ranking the best-selling product categories (e.g., Bed_Bath_Table, Health_Beauty, Computers_Accessories).
* **Analysis:** Identifies the core product lines driving the company's revenue.
* **Insight:**
    * **"Bed, Bath & Table"** and **"Health & Beauty"** consistently appear as top performers.
    * **Actionable Insight:** These categories are the "Cash Cows" of the platform. Marketing budgets should be optimized to maintain visibility for these high-demand categories.
 
  ![Dashboard1](dashboard1.jpeg)
  
---

## 🚚 Dashboard 2: Logistics & Delivery Efficiency
This dashboard analyzes the supply chain performance, which is critical for e-commerce success in a large country like Brazil.

### 1. Delivery Status: On-Time vs. Late ⏱️
* **Visualization:** Shows the percentage of orders delivered on or before the estimated date vs. those delayed.
* **Analysis:** Based on the calculated field: `IF [Delivery Date] > [Estimated Date] THEN 'Late' ELSE 'On Time' END`.
* **Insight:** Highlights the reliability of the logistics network. A high "Late" percentage in specific periods helps identify bottlenecks in the shipping process.

### 2. Average Delivery Time by State 🚛
* **Visualization:** Compares the average number of days taken to deliver a package across different states.
* **Analysis:** Calculated as `DATEDIFF('day', [Order Approved], [Delivered to Customer])`.
* **Insight:** Reveals regional disparities; states closer to the distribution hubs (South/Southeast) have much faster delivery times compared to remote Northern states, explaining the lower sales volume in those regions.

### 3. Average Freight Value  📦
* **Visualization:** Displays the average shipping cost paid by customers per state.
* **Insight:** High freight costs in remote states are likely a barrier to purchase, negatively impacting conversion rates in those areas.

### 4. Delivery Speed Trend  🏃‍♂️📉
* **Visualization:** Tracks the average number of days taken to deliver orders over time (Monthly trend).
* **Analysis:** Monitors the efficiency of logistics partners throughout the year.
* **Insight:**
    * **Seasonal Bottlenecks:** Shows spikes in delivery times during peak seasons (like Black Friday), indicating that logistics partners struggle to handle high volume.
    * **Operational Improvements:** A downward trend over the years would indicate that the company is successfully optimizing its supply chain and reducing wait times for customers.
 
  ![Dashboard1](dashboard2.jpeg)
---

## ⭐ Dashboard 3: Customer Satisfaction & Reviews
This dashboard connects operational metrics (like shipping) to customer sentiment.

### 1. Customer Satisfaction KPIs 📌
* **Metrics:** Displays the overall **Average Review Score** (out of 5), **Total Number of Reviews**.
* **Insight:**
    * **Brand Health:** Acts as the primary "pulse check" for the business. A score consistently above 4.0 indicates a healthy relationship with customers.
    * **Engagement:** The total volume of reviews shows how active and engaged the customer base is with the platform.
    * 
### 1. Review Score Distribution  📊
* **Visualization:** A count of orders by Review Score (1 to 5 stars).
* **Analysis:** Shows the overall customer sentiment profile.
* **Insight:** The majority of customers give **5-star ratings**, indicating general satisfaction. However, the volume of 1-star ratings is significant enough to warrant investigation.

### 2. Correlation: Delivery Time vs. Review Score  📉
* **Visualization:** Plots the Average Review Score against the Average Delivery Time (in days).
* **Analysis:** Investigates if longer shipping times lead to lower ratings.
* **Insight:** **Strong Negative Correlation:** There is a clear trend where orders with long delivery times (e.g., >15 days) receive significantly lower review scores. This confirms that **Logistics speed is the #1 driver of customer satisfaction** in this market.

### 3. Lowest Rated Product Categories  📉
* **Visualization:** A bar chart ranking product categories starting from the **lowest** Average Review Score to the highest.
* **Analysis:** Identifies specific product lines that consistently disappoint customers.
* **Insight:**
    * **Problem Areas:** Highlights categories (e.g., *Security & Services* or specific *Electronics*) that suffer from quality issues or misleading descriptions.
    * **Actionable Insight:** These "Red Flag" categories require immediate quality control audits or removal from the marketplace to protect the brand's reputation.

### 4. Satisfaction Trend Over Time  📅
* **Visualization:** Tracks the fluctuation of the **Average Review Score** month over month (from 2016 to 2018).
* **Analysis:** Monitors the stability of customer sentiment over the long term.
* **Insight:**
    * **Seasonal Impact:** Often reveals that customer satisfaction **dips during peak seasons**  due to logistics delays, reinforcing the correlation between shipping speed and happiness.
    * **Operational Consistency:** A steady line indicates reliable operations, while sudden drops alert management to systemic failures during specific periods.
 
  ![Dashboard1](dashboard3.jpeg)

  ---
