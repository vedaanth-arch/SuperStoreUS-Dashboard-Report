
# 📊 Power BI Dashboards – Superstore Sales Analysis

This repository contains two Power BI dashboards built using the **Sample Superstore Sales** dataset:

* ✅ Operational Dashboard
* 📈 Sales Performance Dashboard

These dashboards were designed to provide both **real-time monitoring** and **strategic insight** into retail business operations and sales behavior.

---

## 🧾 Dataset Used

**Sample Superstore Sales Dataset**
A fictional dataset that includes orders, shipping details, product categories, and customer segments.
Main fields:

* `Order Date`, `Ship Date`, `Region`, `Category`, `Sales`, `Profit`, `Discount`, `Quantity`, `Segment`, etc.

---

## ✅ 1. Operational Dashboard

### 🎯 Purpose:

To monitor **daily business operations** and provide real-time visibility into key metrics like sales, order volumes, profit, and shipping delays. It helps decision-makers react quickly to ongoing activities.

---

### 📊 Key Visuals & Analytics:

| Visual                              | Description                                                                                                        |
| ----------------------------------- | ------------------------------------------------------------------------------------------------------------------ |
| **KPI Cards**                       | Display total Sales, Profit, Quantity, and Count of Orders (using Count of `Order ID`)                             |
| **Sales Trend (Line Chart)**        | Shows sales performance over time using the `Order Date` field (monthly granularity)                               |
| **Category-wise Sales (Bar Chart)** | Breaks down sales across product categories and sub-categories                                                     |
| **Sales by Region (Map)**           | Visualizes regional distribution of sales                                                                          |
| **Shipping Delay Table**            | Shows delay between `Order Date` and `Ship Date` using a calculated column: `DATEDIFF(Order Date, Ship Date, DAY)` |
| **Slicers**                         | Filters for Segment, Region, Category, Date range                                                                  |

---

### 📈 Key Outcomes:

* Found that **Technology** category generated the highest daily sales volume.
* Identified **delays in standard shipping** across the East region.
* Helped simulate real-time alerts for high-profit but low-order volume regions.
* Useful for **day-to-day performance monitoring** and **logistics coordination**.

---

## 📈 2. Sales Performance Dashboard

### 🎯 Purpose:

To analyze **sales trends**, **product performance**, and **customer segmentation** over a longer period to guide strategic planning and performance evaluation.

---

### 📊 Key Visuals & Analytics:

| Visual                                         | Description                                                                                                                 |
| ---------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------- |
| **KPI Cards**                                  | Shows Total Sales, Total Orders (Count of `Order ID`), and Average Order Value (AOV = `SUM(Sales)/DISTINCTCOUNT(Order ID)`) |
| **Sales Trend Over Time (Line Chart)**         | Displays month-over-month sales using `Order Month` column                                                                  |
| **Top Products/Sub-Categories (Bar Chart)**    | Highlights top 10 performing products or sub-categories                                                                     |
| **Sales by Segment & Region (Stacked Column)** | Compares revenue by customer segment across regions                                                                         |
| **TreeMap – Category Breakdown**               | Visualizes the contribution of each product category to overall sales                                                       |
| **Product Table View**                         | Tabular view of `Product Name`, `Sales`, `Quantity`, and `Profit` for detailed analysis                                     |
| **Slicers**                                    | Segment, Region, Category, Date Range filters for dynamic insights                                                          |

---

### 📈 Key Outcomes:

* Revealed that **Corporate segment** had higher AOV compared to the Consumer segment.
* **Furniture** category showed low profit margins despite high sales — indicating a need to re-evaluate pricing or discount strategies.
* Helped identify **top-performing products** by sales and profit.
* Ideal for **strategic sales planning**, **product portfolio optimization**, and **market targeting**.

---

## 🧠 Business Value & Decision-Making Impact

| Operational Dashboard                                           | Sales Performance Dashboard                                                         |
| --------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| Helps monitor business on a daily/weekly basis                  | Helps in long-term planning and sales strategy                                      |
| Useful for teams like logistics, operations, customer service   | Useful for leadership, sales managers, and marketing teams                          |
| Enables quick decisions on bottlenecks, delays, or order spikes | Enables data-driven decisions on product focus, regional investment, and promotions |

---

## 🛠 Tools Used

* **Power BI Desktop**
* DAX (for measures like AOV, Shipping Delay)
* Data modeling and relationships
* Interactive slicers and custom visual formatting

---

## 📎 Conclusion

These dashboards demonstrate how even a simple dataset like Superstore Sales can generate **meaningful insights** through data visualization.
Whether it's tracking real-time metrics or analyzing high-level sales trends, Power BI provides a powerful platform to support **data-driven decisions**.
