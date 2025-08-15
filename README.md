# PowerBI_Practical_Exam_-Abdirisak-
# Retail Sales Analysis – Power BI Project

## 📌 Project Overview
This project analyzes a fictional retail sales dataset designed to demonstrate end-to-end data modeling, visualization, and insights generation in **Power BI**.  
The dataset contains **10,000+ records** spread across the following tables:

- **Sales**: Order details including date, product, customer, quantity, and sales amount.
- **Products**: Product names, categories, subcategories, and cost information.
- **Customers**: Customer demographic data including city, state, and country.
- **Dates**: Date dimension table with hierarchical fields for drill-down (Year, Quarter, Month, Day).
- **Geography**: Location mapping table with city, state, country, and region.

The goal was to build an **interactive sales dashboard** with drill-down functionality from country → state → city, while also enabling insights on product performance, customer distribution, and time-based trends.

---

## 🛠️ Approach

1. **Dataset Creation**
   - Used a structured schema matching the required columns.
   - Established relationships in Power BI between `Sales`, `Products`, `Customers`, `Dates`, and `Geography`.

2. **Data Modeling**
   - Implemented a **star schema** with `Sales` as the fact table and all other tables as dimensions.
   - Created calculated columns and measures for:
     - Total Sales
     - Total Quantity Sold
     - Profit (SalesAmount - Cost)
     - Year-over-Year Growth
     - sales category

3. **Data Visualization**
   - Built an **interactive map visual** with drill-down capability from Country → State → City.
   - Created:
     - Sales trends over time
     - Top product categories
     - Regional performance analysis
     - Customer distribution
   - Applied slicers for filtering by year, product category, and region.

4. **Publishing**
   - Published the Power BI report to **Power BI Service**.
   - Configured a shareable link for stakeholders to interact with the dashboard online.

---

## 🚧 Challenges & Solutions

| Challenge | Solution |
|-----------|----------|
| **Map drill-down to cities** | Created a dedicated `Geography` table with consistent city, state, and country mappings, ensuring it linked correctly to the `Customers` table. |
| **Performance with 10,000+ rows** | Optimized model by removing unused columns and applying data types efficiently. |
| **Publishing & sharing** | Ensured report was published to the Power BI Service with public access link enabled for easy stakeholder viewing. |

---


---

## 🔗 Live Power BI Report
[**Click here to view the interactive dashboard**](https://app.powerbi.com/view?r=YOUR_REPORT_LINK_HERE)

---

## 📁 Repository Structure
