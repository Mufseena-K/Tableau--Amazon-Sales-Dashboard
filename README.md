# Tableau--Amazon-Sales-Dashboard
# Amazon Sales and Logistic Performance

## 1. Project Overview

### 1.1 Project Title
**Amazon Sales and Logistic Performance**

### 1.2 Objective
The project aims to analyze Amazon order delivery performance, order fulfillment efficiency, and customer behavior to optimize logistics and reduce late deliveries and cancellations.

### 1.3 Scope
#### KPIs:
- **Total Orders**
- **Total Revenue**
- **Late Delivery Rate**
- **On-Time Delivery Rate**
- **Cancellation Rate**
- **Average Order Value (AOV)**

### 1.4 Timeline
| Phase             | Description                                      | Estimated Duration |
|------------------|------------------------------------------------|------------------|
| Data Collection | Gathering relevant datasets                    | 1 day           |
| Data Cleaning   | Handling missing values, removing duplicates   | 2 days          |
| Data Modeling   | Defining relationships, creating measures      | 0 days          |
| Visualization   | Designing dashboard and visual elements        | 2 days          |
| Final Review   | Testing and refining dashboard                 | 1 day           |

---

## 2. Data Collection & Preparation

### 2.1 Data Sources
- Used **Kaggle dataset of Amazon sales** containing **128,942 records** and **14 columns** related to Amazon order fulfillment, shipping, and sales.

### 2.2 Data Cleaning & Transformation
- **Identified Missing Data**: Used Power Query’s "Column Profile" and "Column Distribution" tools to detect null values.
- **Removed Duplicates**: Checked for duplicate orders based on **Order ID, Order Date**.
- **Data Type Standardization**:
  - Ensured all numerical fields were in the correct data type (integer, decimal).
  - Removed unused columns to improve performance.

---

## 3. Dashboard Development

### 3.1 Mockup Designs
- Initial wireframes and sketches were created to visualize the final dashboard layout.

### 3.2 Key Visualizations
#### **KPIs Used:**
- **Total Orders** (Distinct Count of Order ID)
- **Total Sales Amount**
- **Average Order Value (AOV)** = (Total Sales Amount / Number of Orders)
- **Late Delivery Rate** = (Late Deliveries / Total Deliveries) * 100
- **On-Time Delivery Rate** = (On-Time Deliveries / Total Deliveries) * 100
- **Cancellation Rate** = (Cancelled Orders / Total Orders) * 100

#### **Amazon Order Fulfillment & Performance Overview (Dashboard 1)**
- **Order Status Distribution (Pie Chart)**: Displays order proportions (Shipped, Delivered, Cancelled, Returned, Pending).
- **Expedited vs. Standard Orders (Square Chart)**: Shows the proportion of expedited vs. standard orders.
- **Amazon vs. Merchant Fulfillment Performance (Bar Chart)**: Compares Amazon vs. third-party merchant fulfillment.
- **B2B vs. B2C Orders (Bubble Chart)**: Shows the share of B2B vs. B2C sales.

#### **Amazon Logistics & Sales Performance (Dashboard 2)**
- **Total Sales by Region (Map)**: Visualizes total sales across different regions.
- **Late Deliveries by Region (Treemap)**: Highlights areas with high late deliveries.
- **Top 10 Cities by Order Volume/Revenue (Bar Chart)**: Displays highest order and revenue-generating cities.
- **Cancellation Rate by Location (Bar Chart)**: Highlights areas with high cancellations.
- **Fulfillment Performance by Category (Bubble Chart)**: Displays fulfillment success rates across product categories.

### 3.3 Measures and Calculations
- **Total Orders** = DISTINCTCOUNT(Order ID)
- **Total Sales Amount** = SUM(Sales Amount)
- **Average Order Value (AOV)** = Total Sales Amount / Number of Orders
- **Late Delivery Rate** = (Late Deliveries / Total Deliveries) * 100
- **On-Time Delivery Rate** = (On-Time Deliveries / Total Deliveries) * 100
- **Cancellation Rate** = (Cancelled Orders / Total Orders) * 100

### 3.4 Filters and Slicers
- **Fulfillment Slicer**: Used in "Amazon Order Fulfillment & Performance Overview".
- **Category Filter**: Used in "Amazon Logistics & Sales Performance".

---

## 4. Insights & Findings

### **Expedited vs. Standard Orders**
- **Expedited Orders:** 68.89% (preferred by customers).
- **Standard Orders:** 31.11% (contributing to late deliveries).
- **Actionable Insight:** Expand expedited shipping options.

### **Fulfillment Performance: Amazon vs. Merchant**
- **Amazon Fulfillment:** 69.78% of orders, more efficient.
- **Merchant Fulfillment:** 30.22%, facing logistical issues.
- **Decision Impact:** Shift more fulfillment to Amazon warehouses.

### **B2B vs. B2C Market Segmentation**
- **B2C Orders:** 99.15% of total sales.
- **B2B Market:** Less than 1%.
- **Decision Impact:** Explore B2B opportunities via partnerships and bulk discounts.

### **Sales Performance & Revenue Trends**
- **Total Sales:** ₹78.57 million, AOV: ₹653.
- **Top Cities:** Bengaluru (11,096 orders), followed by Hyderabad & Mumbai.
- **Top-Selling Regions:** Maharashtra, Karnataka, Tamil Nadu.
- **Actionable Insight:** Optimize inventory in high-demand regions.

### **Late Deliveries & Logistics Efficiency**
- **Overall Late Delivery Rate:** 3.07%.
- **Worst-Affected Regions:** Mizoram (25%), Ladakh (14.29%), Puducherry (14.46%).
- **Actionable Insight:** Improve courier efficiency and establish regional warehouses.

### **Order Cancellations & Returns**
- **Cancellation Rate:** 14.21%, highest in Rajasthan (33.33%) and Lakshadweep (25%).
- **Actionable Insight:** Investigate and reduce cancellation causes.

---

## 5. Challenges & Limitations
- **Dataset Constraint:** Contains only one unique date, limiting time-based analysis.
- **Tool Complexity:** Tableau’s interface is more complex compared to Power BI.

---

## 6. Future Enhancements
- Incorporate **historical data** for trend analysis.
- Optimize **chart types** for better readability.
- Add **tooltips & annotations** to enhance insights.

---

## 7. Conclusion
This project provides actionable insights into order fulfillment, sales performance, and logistics efficiency, enabling businesses to optimize operations and improve customer satisfaction.

### **Key Takeaways:**
- **Late Deliveries & Logistics Challenges:** Suggested regional fulfillment centers & better courier partnerships.
- **High Cancellation & Return Rates:** Identified key problem areas & suggested solutions.
- **Amazon vs. Merchant Fulfillment:** Found Amazon to be more efficient; recommended process improvements.
- **Sales & Customer Insights:** Highlighted top-performing regions & underutilized B2B potential.
- **Decision-Making Through Data Visualization:** Created interactive dashboards for tracking KPIs & improving business strategies.

---

## 8. Appendix
- Data source: **Kaggle Amazon Sales Dataset**
- Tools Used: **Tableau, Power Query**

