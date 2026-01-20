# Customer Churn & Retention Analysis 🏦

## 📌 Project Overview
In the competitive Fintech and Banking sector, customer retention is often more cost-effective than acquisition. This project analyzes **28,000+ customer records** from a multinational bank to identify key indicators of churn. 

Unlike standard demographic analysis, this project focuses on **financial behavioral patterns** (e.g., credit usage, net worth fluctuations, and transaction vintage) to predict high-risk customers.

## 🎯 Key Business Questions
* **Who is leaving?** Identifying churn rates across different Net Worth categories.
* **Why are they leaving?** correlating account balance drops with exit behavior.
* **Who should we save?** Calculated **Customer Lifetime Value (LTV)** to prioritize retention efforts for high-value users.

## 🛠️ Tech Stack
* **Python:** Pandas (Data Cleaning), Scikit-Learn (Random Forest Classification).
* **Power BI:** Interactive Dashboard, DAX Measures (Churn Rate %, Revenue at Risk).
* **SQL:** Data querying and validation logic.

## 📊 Approach & Methodology
1.  **Data Preprocessing:** Handled missing values in the `gender` and `dependent` columns; normalized financial values (Net Worth) for consistent scaling.
2.  **Exploratory Data Analysis (EDA):**
    * Identified that customers with a **significant drop in 'Current Month Credit'** were 3x more likely to churn.
    * Discovered that **"Medium Net Worth"** clients had the highest churn rate (Target Segment).
3.  **Feature Engineering:** Created a `Vintage_Year` flag to analyze long-term loyalty vs. new customer churn.
4.  **Predictive Modeling:** Built a Random Forest Classifier to predict churn probability.
5.  **Visualization:** Designed a Power BI Executive Dashboard to track "Revenue at Risk."

## 📈 Key Findings (Dashboard Insights)
* **Churn Rate:** The overall churn rate for the analyzed period was **18.5%**.
* **Risk Signal:** Customers whose account balance dropped below **₹5,000** showed an **80% probability** of churning within the next 30 days.
* **Financial Impact:** Identified **₹45M in Revenue at Risk**, allowing the business to focus retention budget on the top 10% of high-LTV customers.

## 📸 Dashboard Preview
*(A visual representation of the Churn Analysis and LTV segments)*

![Dashboard Screenshot](Dashboard_Screenshot.png)

## 📂 Repository Structure
* `churn_analysis.py`: Python script for data cleaning, EDA, and Random Forest modeling.
* `Bank_Churn_Dashboard.pbix`: (Optional) The Power BI source file.
* `README.md`: Project documentation.

---
*Note: The dataset used is anonymized financial data ("ABC Multistate Bank") for educational and analytical purposes.*
