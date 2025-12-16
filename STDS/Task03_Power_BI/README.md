**🍕 Pizza Sales Data Analysis Project**

 
This project focuses on performing an in-depth data analysis of pizza sales 🍕 to extract Key Performance Indicators (KPIs), understand customer behavior, identify temporal patterns (daily, hourly, and monthly), and support strategic business decisions.

---
**⚙️ Data Preprocessing Stage**
In this stage, the data was prepared to be suitable for analysis, which involved two crucial steps:

1. Extracting Temporal Dimensions ⏰
   
Process: We successfully extracted the Day Name and Month Name columns from the original Order Date column.

Importance: This allowed us to perform deep analysis of seasonal and behavioral patterns daily and monthly, which is clearly demonstrated in charts like Total Orders by Month and Total Orders by Day Name.

2. Modifying Data Types 🧬
   
Process: Adjustments were made to the Data Types of various columns to ensure accurate calculations and correct categorical classification.

3. Covert Sizes Form (S , M, L,XL) to (Small , Meduim , Large , Xlarge)

Importance: This step ensured that numerical columns (like quantities and prices) were stored as numbers, and temporal columns were stored as dates, resulting in accurate calculations and visualizations.

**📈 Interactive Dashboard**

After data preparation, an interactive Dashboard was created to display the results in an accessible and understandable format. The Dashboard includes:

## 📊 Dashboard Overview (Page 1)
The first page of the dashboard serves as a comprehensive **Executive Summary**. It provides a high-level view of the business performance, focusing on revenue, volume, and customer trends over time.

### 1. Key Performance Indicators (KPIs) 📌
these cards provide immediate visibility into the store's core metrics:
* **Total Revenue:** The sum of the total price of all pizza orders.
    * *Insight:* Indicates the overall financial health and total earnings of the business.
* **Average Order Value:** The average amount spent by a customer per transaction.
    * *Insight:* Helps in understanding customer spending behavior and evaluating pricing strategies.
* **Total Pizzas Sold:** The total quantity of pizzas sold across all categories.
    * *Insight:* Measures the production volume and demand.
* **Total Orders:** The total count of distinct orders placed.
    * *Insight:* Tracks the traffic and customer volume.
* **Avg Pizzas Per Order:** The average number of pizzas contained in a single order.
    * *Insight:* Reveals purchase patterns (e.g., are customers buying for groups or individuals?).


### 2. Sales by Pizza Category 
* **Visualization:** Break down of total sales revenue by pizza category (Classic, Supreme, Chicken, Veggie).
* **Analysis:** Shows the percentage contribution of each category to the total revenue.
* **Insight:** **Classic** category contributes the most to sales, suggesting it contains the most popular menu items, while other categories may need promotional boosts.

### 3. Sales by Pizza Size 
* **Visualization:** Break down of total sales revenue by pizza size (S, M, L, XL, XXL).
* **Analysis:** Shows which pizza sizes are generating the most revenue.
* **Insight:** **Large (L)** size pizzas account for the highest percentage of sales, indicating that customers perceive the Large size as the best value for money or are ordering for groups.

### 4. Top 5 Best-Selling Pizzas 
* **Visualization:** A set of bar charts ranking the top 5 pizza types based on **Revenue**.
* **Analysis:** Highlights the "Star" products of the menu.
* **Insight:**
    * **The Thai Chicken Pizza** contributes the highest revenue.
    * **Actionable Insight:** These top performers must always remain in stock. The business should focus marketing efforts on these items and consider bundling them with lower-selling items to boost overall sales.

### 5. Bottom 5 Worst-Selling Pizzas 
* **Visualization:** A set of bar charts identifying the 5 least popular pizza types based on **Revenue**.
* **Analysis:** Flags underperforming menu items that are generating the least financial return.
* **Insight:**
    * **The Brie Carre Pizza** is consistently at the bottom  on Revenue.
    * **Actionable Insight:** These items might need re-evaluation. The business could consider running special promotions to clear inventory, improving the recipe, or removing them from the menu entirely to reduce waste and operational complexity.

![dashdoard 1 ](dashboard.PNG)

---

### 1. Busiest Days & Hours (Heatmap / Matrix) 
**Visualization**: A matrix view plotting Days of the Week against Hours of the Day, with the values representing the volume of Total Orders.
* **Analysis:** : This chart helps visualize traffic density. Darker or higher values indicate peak rush hours, while lighter values indicate slow periods.

* **Insight:** Peak Times: Identifies specific time slots (e.g., Thursday/Friday evenings from 6 PM to 9 PM) where the store experiences the highest demand.

* **Actionable Insight:** Crucial for Staffing & Operations. Managers can use this data to schedule more staff and prepare more dough during these specific windows to reduce wait times, and reduce staff during low-traffic hours (e.g., weekdays before 12 PM) to save costs.
* 
### 2. Daily Trend for Total Orders 
* **Visualization:** Displays the distribution of total orders across different days of the week.
* **Analysis:** Aggregates order volume by day (Sunday to Saturday).
* **Insight:** Identifies the busiest days of the week. Typically, **Fridays** show the highest traffic, indicating a need for increased staff and inventory during weekends.

### 3. Monthly Trend for Total Orders 
* **Visualization:** Tracks the total number of orders across different months of the year.
* **Analysis:** Shows the fluctuation in sales volume from January to December.
* **Insight:** Highlights seasonal patterns and peak periods (e.g., spikes during holiday seasons or summer months), aiding in long-term resource planning.

### 4. Hourly Trend for Total Orders 
* **Visualization:**  A line chart representing the volume of orders placed during each hour of the day (from opening to closing time).
* **Analysis:**  Provides a continuous view of customer traffic flow throughout the operational hours.
* **Insight:**  Lunch & Dinner Rushes: Typically reveals two major spikes: one around 12:00 PM - 1:00 PM (Lunch) and a larger peak between 5:00 PM - 8:00 PM (Dinner).

* **Operational Planning:** Helps managers anticipate exact "rush hours" to ensure fresh food preparation aligns with demand, minimizing wait times.

### 5. Monthly Orders vs. Target (Gauge Chart) 
* **Visualization:**  A gauge meter comparing the Current Total Orders (or Revenue) against a pre-set Monthly Target (Goal).
* **Analysis:**  Acts as a visual "progress bar" for the business objectives.
* **Insight:** Performance Tracking: Instantly shows if the store is "On Track" (Green) or "Behind Target" (Red) for the month.
* **Motivation:** Serves as a quick health check for the sales team to push for more sales if the needle hasn't hit the target yet.  

![dashdoard 2 ](dashboard1.PNG)

---
