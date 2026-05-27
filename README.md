## Bicycle Retail Sales Analytics Case Study 

*Executive Sales Dashboard: 2016-2018 Performance Analysis* 

**Executive Summary** 

This case study presents a comprehensive data analytics project that transforms raw sales data from a bicycle retail company into actionable business intelligence. Through an integrated workflow utilizing SQL, Microsoft Excel, and Tableau, the project delivers interactive dashboards that enable executive leadership to monitor sales performance, identify revenue trends, and make data-driven strategic decisions. 

The analysis covers three years of sales activity (2016-2018) and provides critical insights into revenue patterns across multiple dimensions: geographic regions, store locations, product categories, brand performance, customer behavior, and sales representative effectiveness. The project demonstrates end-to-end data analytics capabilities from database extraction through interactive visualization. 

**Business Context and Objectives** 

**The Challenge** 

Company leadership required comprehensive visibility into sales operations but faced a critical challenge: traditional static reports were too lengthy, difficult to navigate, and provided limited analytical flexibility. Decision-makers needed a solution that would allow them to quickly explore data, identify trends, and drill down into specific metrics without requesting new reports for every question. 

**Key Business Questions** 

The executive team sought answers to critical strategic questions: 

● What are the overall sales volume trends from 2016 through 2018? Are we growing or declining? 

● Which geographic regions and individual stores generate the highest revenue? ● Which product categories and brands drive the most sales? 

● Who are our most valuable customers, and how much revenue do they contribute? ● Which sales representatives are top performers, and what can we learn from their success? 

● Are there seasonal patterns or monthly trends that should inform inventory and staffing decisions? 

**The Solution** 

Rather than delivering static reports, this project provides interactive dashboards that empower executives to explore data dynamically. Users can filter by year, region, or store with a single click, instantly updating all visualizations to reflect their selected criteria. This self-service approach reduces dependency on data analysts and accelerates decision-making. 

**Methodology: The Five-Step Data Analytics Process** 

This project follows a structured analytical framework that ensures comprehensive, accurate, and actionable results: 

**Step 1: Understand the Problem** 

Collaborated with stakeholders to define business objectives, identify key performance indicators (KPIs), and establish dashboard requirements. Determined that the analysis should focus on revenue metrics, sales trends, and comparative performance across regions, stores, products, and personnel. 

**Step 2: Collect the Data** 

Extracted data from the company's relational database, which stores information across multiple interconnected tables in sales and production schemas. Developed SQL queries to consolidate data from nine related tables, ensuring all necessary fields were captured for analysis. 

**Step 3: Clean and Prepare the Data** 

Validated data quality by checking for missing values, duplicates, and inconsistencies. Standardized naming conventions by concatenating first and last names for customers and sales representatives. Calculated derived metrics such as total units sold and revenue per transaction. Ensured data types were properly formatted for analysis and visualization. 

**Step 4: Analyze and Visualize** 

Created pivot tables and charts in Excel to explore initial patterns and relationships. Developed interactive dashboards with filtering capabilities to enable dynamic exploration. Built advanced Tableau visualizations with rich interactivity, including geographic maps, trend lines, and comparative charts. 

**Step 5: Interpret and Communicate Results** 

Translated data findings into business insights with clear, executive-friendly visualizations. Designed dashboards that tell a coherent story about company performance while allowing users to investigate specific areas of interest. Documented key findings and recommendations for strategic action. 

**Technical Implementation** 

**Data Architecture and SQL Extraction** 

The company's sales data resides in a normalized relational database with separate tables for orders, customers, products, categories, brands, stores, and staff. This structure, while efficient for transactional processing, required complex joins to create an analytical dataset. 

**SQL Approach** 

The extraction strategy involved: 

● Joining nine related tables from sales and production schemas to create a unified dataset 

● Using CONCAT functions to merge first and last names into single customer and sales representative fields 

● Applying aggregate functions (SUM) to calculate total units sold and revenue per order 

● Calculating revenue as the product of quantity and list price for each order item ● Grouping results by order, customer, location, date, product, and sales representative ● Filtering data to include only transactions from 2016 through 2018 

**Key Fields in the Dataset** 

The resulting analytical dataset includes the following dimensions and metrics: 

| Field Category  Order Information  | Fields  Order ID, Order Date |
| :---- | :---- |
| **Customer Information**  | Customer Name, City, State |
| **Product Information**  | Product Name, Category, Brand |
| **Store Information**  | Store Name, Location |
| **Sales Information**  | Sales Representative Name |
| **Metrics**  | Total Units Sold, Revenue (Quantity × List Price) |

**Excel Dashboard Development** 

Microsoft Excel serves as the first visualization layer, providing accessible, familiar tools for data exploration. The Excel dashboard leverages pivot tables, charts, and interactive slicers to create a dynamic analytical environment. 

**Data Integration** 

The SQL-generated dataset was imported into Excel using a direct database connection rather than static file imports. This approach ensures that the dashboard automatically refreshes whenever the underlying database is updated, maintaining data currency without manual intervention. 

**Visualizations Created** 

**Column Chart \- Annual Revenue:** Displays total revenue for each year (2016, 2017, 2018), enabling quick identification of growth trends 

**Line Chart \- Monthly Revenue Trends:** Shows revenue patterns across 36 months, revealing seasonality and helping forecast future performance 

**Map Chart \- Geographic Distribution:** Visualizes revenue by state using color intensity, instantly highlighting top-performing and underperforming regions 

**Pie Chart \- Store Performance:** Illustrates each store's contribution to total revenue, facilitating resource allocation decisions 

**Bar Charts \- Category and Brand Analysis:** Compares revenue across product categories and brands, identifying which offerings drive the most sales 

**Column Chart \- Top 10 Customers:** Ranks the highest-value customers, supporting targeted retention and loyalty programs 

**Bar Chart \- Sales Representative Performance:** Shows revenue generated by each sales representative, enabling performance recognition and best practice sharing 

**Interactive Features** 

The Excel dashboard incorporates slicers for Year, State, and Store Name. When a user selects a filter option, all charts automatically update to reflect only the selected data. This interactivity transforms the dashboard from a static report into an exploratory tool that answers questions on demand. 

**Tableau Dashboard Development** 

While Excel provides solid analytical capabilities, Tableau offers advanced visualization features and superior design aesthetics for executive presentations. The Tableau dashboard builds upon the Excel foundation with enhanced interactivity and more sophisticated visual techniques. 

**Design Principles** 

The Tableau implementation prioritizes clean, professional design: revenue displayed in currency format without decimals, gridlines removed for visual clarity, and color schemes chosen for both aesthetics and accessibility. Each visualization answers a specific business question while contributing to the overall narrative. 

**Advanced Features** 

**Tree Map Visualization:** Used for product category analysis, this visualization efficiently displays multiple categories simultaneously without cluttering the dashboard. Rectangle size represents revenue contribution, making top categories immediately obvious. 

**Dynamic Top N Parameter:** Allows users to select how many top customers to display (e.g., Top 5, 10, or 20). This flexibility accommodates different analytical needs without requiring separate reports. 

**Action Filters:** Custom worksheets function as interactive year and state filters. Clicking on a year or state in these worksheets instantly filters all other visualizations, creating a seamless exploration experience. 

**Geographic Maps with Color Gradients:** State-level revenue displayed on an interactive map with color intensity indicating performance levels. Users can immediately identify geographic patterns and opportunities. 

**Key Findings and Business Insights** The dashboards reveal several critical insights that inform strategic decision-making: 

**Revenue Trends and Growth Patterns** 

Analysis of the three-year period shows clear trends in overall revenue trajectory and monthly patterns. The line chart visualization reveals seasonal fluctuations that should inform inventory planning and staffing decisions. Specific months demonstrate consistent peaks and valleys, suggesting opportunities for targeted marketing campaigns during slower periods and capacity planning during high-demand months. 

**Geographic Performance Insights** 

The map visualization reveals significant geographic variation in sales performance. New York consistently generates the highest revenue across all three years, while Texas shows the lowest regional performance. These findings suggest several strategic questions: Does New York's success reflect market size, competitive positioning, or superior execution? What factors contribute to underperformance in Texas, and can successful practices from top regions be replicated elsewhere? 

**Product and Brand Performance** 

The category and brand analysis identifies Trek as the most profitable brand, significantly outperforming competitors. This insight has direct implications for inventory management, supplier relationships, and marketing strategy. The company should ensure adequate Trek inventory during peak seasons and consider expanding the Trek product line. Simultaneously, leaders should investigate whether underperforming brands face product quality issues, pricing problems, or simply lack adequate promotion. 

**Customer and Sales Representative Performance** The Top 10 customers chart reveals significant revenue concentration among a small group of high-value clients. This finding highlights the importance of customer retention strategies and account management for key relationships. Sales representative analysis shows top performers like Marceline Boyer and Venita Daniel consistently generating higher revenue than their peers. Understanding what makes these representatives 

successful—whether relationship-building skills, product knowledge, or territory advantages—could inform training programs and best practice sharing. 

**Project Deliverables** 

**1\. SQL Script:** Comprehensive query that extracts and transforms data from nine related database tables into a unified analytical dataset. The script includes joins, aggregations, and calculated fields necessary for analysis. 

**2\. Excel Dashboard:** Interactive workbook containing pivot tables, charts, and slicers. Users can filter data by year, state, or store and see all visualizations update automatically. Includes summary KPIs for total revenue, units sold, and customer counts. 

**3\. Tableau Dashboard:** Professionally designed, highly interactive visualization with advanced features including geographic maps, tree maps, dynamic Top N parameters, and action filters. Optimized for executive presentations and strategic planning sessions. 

**4\. Documentation:** This comprehensive case study document explaining methodology, technical approach, and business insights derived from the analysis. 

**Technology Stack** 

**SQL (SQL Server):** Data extraction, table joins, aggregations, and calculated field creation 

**Microsoft Excel:** Pivot table analysis, chart creation, dashboard design, and slicer-based interactivity 

**Tableau:** Advanced visualization, geographic mapping, action filters, parameter controls, and executive-level presentation design 

**Strategic Recommendations** 

1\. Implement customer loyalty programs focused on the Top 10 revenue-generating customers to strengthen relationships and increase retention rates. 

2\. Analyze success factors behind top-performing sales representatives (Marceline Boyer, Venita Daniel) and develop training programs to share best practices across the entire sales team. 

3\. Investigate the root causes of underperformance in Texas. Consider market research, competitive analysis, or adjustments to product mix, pricing, or marketing strategies in that region. 

4\. Prioritize Trek inventory management given its dominant revenue contribution. Strengthen supplier relationships and ensure adequate stock levels, particularly during peak sales months. 

5\. Develop seasonal marketing campaigns to address monthly revenue fluctuations. Increase promotional activity during consistently slow months to smooth demand patterns. 

6\. Automate dashboard refreshes by maintaining the direct database connection in Excel and scheduling regular data updates in Tableau. This ensures leadership always has access to current information for real-time decision-making. 

7\. Consider expanding the analysis to include profitability metrics (not just revenue) if cost data becomes available. High revenue does not always equal high profit, and margin analysis could reveal different strategic priorities. 

**Conclusion** 

This case study demonstrates the complete data analytics lifecycle, from defining business requirements through delivering actionable insights via interactive dashboards. By leveraging SQL for data extraction, Excel for accessible analysis, and Tableau for executive-level visualization, the project transforms raw transactional data into strategic intelligence. 

The dashboards provide company leadership with unprecedented visibility into sales performance across multiple dimensions. Rather than waiting for periodic reports, executives can now explore data on demand, asking and answering their own questions through intuitive filtering and visualization. This self-service capability accelerates decision-making and enables more data-driven strategic planning. 

The insights revealed—from geographic performance patterns to sales representative effectiveness—create clear pathways for operational improvements and strategic initiatives. By continuing to monitor these metrics through the dashboards and taking action on the recommendations provided, the company can optimize sales performance, strengthen customer relationships, and drive sustainable revenue growth. 

Most importantly, this project establishes a framework and methodology that can be replicated for other analytical initiatives. The five-step process, technical approaches, and dashboard design principles demonstrated here provide a template for future data analytics projects across the organization. 
