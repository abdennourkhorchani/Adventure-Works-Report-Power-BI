# Adventure-Works-Report-Power-BI

This Power BI project provides a comprehensive analysis of Adventure Works sales data, leveraging a snowflake schema data model. The report incorporates bookmarks, drill-through capabilities, and interactive buttons to provide users with flexible and insightful data exploration.

**Project Goals:**

- Gain a holistic view of overall sales performance across key metrics (orders, revenue, profit,returns).
- Identify regional and product-level sales trends.
- Monitor key performance indicators (KPIs) such as monthly revenue, order volume, and return rates.
- Analyze the sales results of individual products/customers.
- Track product performance against sales targets.
- Understand customer demographics and preferences.
  
**Key Features:**

 **Overview Page:**

- Visualizations for total orders, profit, revenue by region, category, and product.
- Monthly trends for revenue, orders and returns.
- Identifies top products by profit and orders using a date and region slicer.

**Product Drill-Through:**

- Detailed product information including average price, price adjustments
- Track current month orders and revenue against target.
- Monitor weekly profit vs adjusted profit after price adjustment.
- Visualize forecasted weekly profit.
- Track weekly return volume over time.

**Customer Page:**

- Visualize orders distribution by income level, gender, occupation and age .
- Analyze orders volume and total revenue of individual customers.
- Identify Top customer and their revenue and total orders.

**Technical Details**

 *  **Data Model:**  A snowflake schema Model is used to organize the data, with 2 fact tables (AW_Sales, AW_Returns) and the following dimension tables:
  
  AW_Calendar_Lookup, AW_Customer_Lookup, AW_Territories_Lookup, AW_Product_Lookup, AW_Product_Subcategory and AW_Product_Cateogry.
   
  Each dimension table is connected to the fact table through a 1-to-many relationship (screenshot in the repository). Product,Subcategory and Cateogry dimensions are connected creating a hierarchical structure.
  
 * **DAX Measures:** Several DAX measures are created to calculate key metrics, such as monthly revenue/profit/returns, total orders/profit, profit adjustment due to price adjustment, top product/customer ...
 * **Visualizations:** The report includes various visualizations, including treemap,matrix,line chart, gauge, KPI, map area, donut and stacked bar chart.
 * **Slicers:** Allow users to drill down into specific data segments by date and region.
 * **Drill-Down Capabilities:** Explore data at different levels of granularity (hierarchies) : Category, subcategory and product.
 * **Drill-through Capabilities:** Navigate from an overview report to a more detailed report page focused on a specific data point (product drill through)
* **Bookmarks:** Create dynamic and interactive reports that guide users through different insights by using 2 bookmarks that save specific states of the report, including filter selections, visual configurations, and page views( exec summary, product detail).

* **Edit Interactions:** Customize how the visualizations on the report page filter and highlight each other. For example monthly revenue,orders,returns do not interact with date slicer.

* **Workspace:** Create a content container that hold dashboards, reports, datasets, and provide a single location to work together on this project.

![Capture](https://github.com/user-attachments/assets/82d67609-69a0-4325-8c86-21b0db07acf2)


* **Publish the report:** Upload the report to the created workspace(Adventure Works Sales).


* 
 **How to Use:**
 Follow the demo video to know how to use the report well.
 

**Future Enhancements**

* **Predictive Analytics:** Implement predictive models to forecast future sales trends, identify potential demand surges, and optimize inventory levels.
* **Integration with Other Systems:** Integrate the dashboard with other business systems, such as CRM, ERP, and marketing automation platforms, to provide a more holistic view of business operations.
* **Content update:** Consider adding additional visualizations or metrics based on specific business needs.
* **Data Pipelines:** Automate data extraction, transformation, and loading (ETL) processes to ensure data freshness and reduce manual effort.


This project enables users to gain valuable insights into sales performance, identify key trends, and make data-driven decisions.

