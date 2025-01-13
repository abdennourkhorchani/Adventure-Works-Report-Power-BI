# Adventure-Works-Report-Power-BI

This Power BI project provides a comprehensive analysis of Adventure Works sales data, leveraging a snowflake schema data model. The report incorporates bookmarks, drill-through capabilities, and interactive buttons to provide users with flexible and insightful data exploration.

**Project Goals:**

- Gain a holistic view of overall sales performance across key metrics (orders, revenue, profit,returns).
- Identify regional and product-level sales trends.
- Monitor key performance indicators (KPIs) such as monthly revenue, order volume, and return rates.
- Analyze the profitability of individual products.
- Identify areas for price optimization and cost reduction.
- Track product performance against sales targets.
- Understand customer demographics and preferences.
  
**Key Features:**

 **Overview Page:**

- Visualizations for total orders, profit, revenue by region, category, and product.
- Monthly trends for revenue, orders, returns, and returns rate.
- Identifies top products by profit and orders using a date and region slicer.

**Product Drill-Through:**

- Detailed product information including average price, price adjustments
- Track current month orders and revenue against target.
- Monitor weekly total profit vs adjusted profit after price adjustment.
- Visualize forecasted weekly profit.
- Track weekly return volume over time.

**Customer Page:**

- Visualize orders distribution by income level, gender, occupation, age .
- Analyze orders volume and total revenue of individual customers.
- Identify Top customer and their revenue and total orders.

**Interactive Features:**
  
Dynamic Filtering: A powerful combination of buttons and bookmarks with slicers and drill through capabilities enables users to quickly filter data by territory, time, category and product providing a dynamic and engaging experience.

- Slicers : Allow users to filter data based on specific criteria.
- Bookmarks : Save specific report states for quick access.
- Drill through : Navigate from an overview report to a more detailed report page focused on a specific data point.
- Drill down : explore data at increasingly granular levels within the same visual.

**Technical Details**

  **Data Model:**
  
  A snowflake schema Model is used to organize the data, with 2 fact tables (AW_Sales, AW_Returns) and the following dimension tables:
  
  AW_Calendar_Lookup, AW_Customer_Lookup, AW_Territories_Lookup, AW_Product_Lookup, AW_Product_Subcategory and AW_Product_Cateogry.
   
  Each dimension table is connected to the fact table through a 1-to-many relationship (screenshot in the repository). Product,Subcategory and Cateogry dimensions are connected creating a hierarchical structure.
  
  **DAX Measures:** Several DAX measures are created to calculate key metrics, such as monthly revenue/profit/returns, total orders/profit, profit adjustment due to price adjustment, top product, customer ...
  **Visualizations:** The report includes various visualizations, including treemap,matrix,line chart, gauge, KPI, map area, donut and stacked bar chart.
  **Slicers:**  slicers allow users to drill down into specific data segments by date and region.
  **Drill-Down Capabilities:** Explore data at different levels of granularity (hierarchies) : Category, subcategory and product.
  **Drill-through Capabilities:** described above
Bookmarks: Create dynamic and interactive reports that guide users through different insights by using 7 bookmarks that save specific states of the report, including filter selections, visual configurations, and page views( clear filter, Users ON/OFF, Currency ON/OFF, Territory ON/OFF).

Edit Interactions Customize how the visualizations on the report page filter and highlight each other. For example total sales last month and total sales amount cards do not interact with currency slicer.

Visualizations: The report includes various visualizations, including line and stacked column chart, card visuals, map chart and table.

Workspace: create a content container that hold dashboards, reports, datasets, dataflows, and paginated reports, and provide a single location to work together on this project.

Publish the report: upload the report to the created workspace(Sales).




* **Profit forecasting:**

* 
 **How to Use:**
 Follow the demo video to know how to use the report well.
 

**Future Enhancements**

* **Predictive Analytics:** 
* **Advanced Analytics:** 
* **Integration with Other Systems:** Integrate the dashboard with other systems.

Content update: Consider adding additional visualizations or metrics based on specific business needs.
Update the data source: Replace getting data from local excel file with a connection to sql server.
Data Refresh: Schedule data refreshes to keep the report up-to-date using a gateway.
Permissions: Control who can view and edit the report by creating roles and adjusting permissions in the workspace settings.


This project enables users to gain valuable insights into sales performance, identify key trends, and make data-driven decisions.


This Power BI project provides a comprehensive analysis of Adventure Works sales data.

