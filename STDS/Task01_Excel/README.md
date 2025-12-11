# 💼 Data Science Jobs Analysis: From Raw Data to Insightful Dashboard

---

## 🔍 Dataset Overview

The project utilized a dataset containing various attributes for global Data Science job postings.

| Feature | Description | Initial Status (Raw Data) |
| :--- | :--- | :--- |
| `post_date` | Date of the job posting. | Needs standardization. |
| `headquarter` | Location of the company headquarters. | Clean. |
| `industry` | Company industry (e.g., Technology, Finance). | Clean. |
| `ownership` | Company ownership (e.g., Public, Private). | Have Missing. |
| `revenue` | Company revenue and status. | **Highly unstructured (Mixed text and numerical values with currency symbols and status).** |
| `Salary` | salary for the job. | **Contained ranges (e.g., 150-170K).** |


---

## 🛠️ Data Pre-processing and Transformation Steps

The core of this project focused on extensive data cleaning and feature engineering to prepare the raw data for accurate analysis.

### 1. Handling Missing Values (Nulls) 🗑️

* **Action:** Missing values (Nulls) across all critical columns were systematically  imputed (most frequent on column [job_title] , "Not Specified" in column [Senority level , statuts]) to ensure the integrity of the statistical calculations.

### 2. Deconstructing the `revenue` Column (Feature Engineering) �

The single, messy `revenue` column was strategically split into two new, clean features:

| New Feature | Purpose | Key Actions |
| :--- | :--- | :--- |
| **`Revenue_numeric`** | The standardized financial value of the revenue. | Cleaned the column by **removing currency symbols** (€, $), converting abbreviations (M, B, T) into full numerical values, and standardizing the data type. |
| **`Revenue Status`** | The reporting status of the company's revenue. | Extracted status details like **'Reported'**, **'Not Reported (Public)'**, and **'Not Defined'** from the original mixed column to create a clean categorical variable. |

### 3. Calculating `AVG_Salary` from Ranges 💰

The original `Salary` column contained salary ranges (e.g., 150705). This required transformation to calculate a meaningful average.

* **Action:** The minimum and maximum values of the salary range were extracted, and a new, single **Average Salary** column was computed. This standardized numerical column is crucial for all subsequent visualizations and comparisons.

---

## 📈 Dashboard Overview & Visual Insights

The dashboard is designed as a two-page interactive report. Each visualization addresses a specific question regarding the Data Science job market in 2025.

### 📊 Dashboard 1: Job Market & Role Analysis
*Focuses on the "Candidate Perspective"—analyzing roles, seniority, and work flexibility.*

#### 1. Average Salary by Job Title (Bar Chart)
* **Visualization:** A comparison of the `AVG_Salary` across different job titles (e.g., Data Scientist, Machine Learning Engineer, Data Analyst).
* **Insight:** Identifies which technical roles command the highest market value( the most is Data Engineer ), helping candidates choose their specialization path.

#### 2. Salary by Work Status (Column Chart)
* **Visualization:** Breaks down the average salary based on the work mode: **Remote**, **On-site**, or **Hybrid**.
* **Insight:** Reveals whether remote positions offer competitive pay compared to office-based roles and how "On site" models are positioned financially.

#### 3. Job Postings by Seniority Level (Bar Chart)
* **Visualization:** Displays the count (volume) of job openings categorized by **Junior**, **Mid-level**, **Senior**, and **Lead** levels.
* **Insight:** Highlights the market demand distribution—showing whether the market is currently hiring more entry-level talent or seeking experienced leaders.

![Dashboard 1](Dashboard1.PNG)

---

### 🏢 Dashboard 2: Company Profile & Industry Economics
*Focuses on the "Employer Perspective"—analyzing how industry and company financial health impact hiring.*

#### 1. Salary Trends by Industry (Bar Chart)
* **Visualization:** Ranks various industries (e.g., Technology, Finance, Healthcare) based on the average salary they offer.
* **Insight:** Pinpoints the most lucrative sectors for Data Scientists to target.

#### 2. Ownership Type Analysis (Pie/Donut Chart) 
* **Visualization:** Compares compensation packages between **Public** (Stock-market listed) and **Private** companies.
* **Insight:** Determines if publicly traded companies, with typically transparent financials, pay significantly more than private entities.

#### 3. Revenue Status Distribution (Chart)
* **Visualization:** Shows the proportion of job postings coming from companies that **report their revenue** vs. those that do not.
* **Insight:** Provides a view of data transparency in the market and correlates established financial reporting with hiring activity.

![Dashboard 2](Dashboard2.PNG)

## 🤝 Conclusion

This project successfully demonstrated end-to-end proficiency in data cleaning (handling nulls, complex extraction) and feature engineering (splitting messy columns) in Excel, concluding with clear, actionable insights through a comprehensive dashboard.

## 💬 Author
**Botayla Amin**  
Data Analyst | Data Scientist

📧 botaylaamin@gmail.com  
