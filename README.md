# **E-Commerce Query Performance Optimization**

## Overview
This project focuses on analyzing the performance of SQL queries in an e-commerce context using the Brazilian E-Commerce Public Dataset from Olist. By implementing various indexing strategies—uninformed, self-optimized, and user-optimized—the project evaluates their impact on query execution times across three different database sizes (small, medium, and large).

## Motivation
In the fast-paced world of e-commerce, where millions of transactions occur daily, the efficiency of database queries plays a pivotal role in ensuring optimal system performance. As data volumes grow, understanding the impact of indexing strategies on query execution times becomes essential for effective database management. This project aims to develop a scalable framework that assesses query performance across various database sizes and indexing methods. By optimizing these queries, we can significantly enhance the responsiveness and reliability of e-commerce platforms, ultimately improving user experience and operational efficiency.

## Dataset Information
- **Source:** [Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)
- **Description:** The dataset comprises 100,000 orders made between 2016 and 2018 across multiple marketplaces in Brazil, offering insights into order status, pricing, payment performance, customer locations, product attributes, and customer reviews.
- **Key Tables:**
  - **Customers:** Contains customer IDs and postal codes.
  - **Sellers:** Contains seller IDs and postal codes.
  - **Orders:** Contains order IDs and customer IDs.
  - **Order Items:** Contains order details (order IDs, item IDs, product IDs, and seller IDs).

## Database Sizes
- **small.db:** ~10k customers, ~500 sellers, ~10k orders, ~2k order items.
- **medium.db:** ~20k customers, ~750 sellers, ~20k orders, ~4k order items.
- **large.db:** ~33k customers, ~1k sellers, ~33k orders, ~10k order items.

## Objectives
1. **Benchmark Query Performance:** Evaluate and compare the execution times of four key SQL queries frequently used in e-commerce platforms across the three database sizes.
2. **Visualize Performance Results:** Create visual representations of query performance, enabling easy comparison and insight into the effectiveness of different indexing strategies.
3. **Database Construction:** Establish a robust testing environment by creating the databases from the Olist dataset, ensuring realistic testing conditions for SQL queries.
4. **Assess SQL Query Efficiency:** Analyze the performance of queries that interact with customer, seller, and order data to demonstrate their efficiency under different indexing scenarios.

## Key Features
- **Performance Comparison:** Execute and measure the performance of SQL queries under uninformed, self-optimized, and user-optimized indexing scenarios.
- **Visualization:** Generate visualizations (e.g., bar plots) to illustrate query performance across the three database sizes.
- **SQL Queries:** Incorporate four distinct SQL queries that reflect key business questions in an e-commerce context.

## Skills Demonstrated
- **Data Analysis:** Apply performance benchmarking and optimization techniques relevant to e-commerce data.
- **SQL Proficiency:** Showcase advanced SQL skills through the formulation of complex queries and application of indexing strategies.
- **Data Visualization:** Use Matplotlib and other libraries to effectively present query performance results and insights.

## Libraries Used
- **Python:** Primary programming language for scripting and executing SQL queries.
- **SQLite:** Database management system for creating and managing the databases.
- **Matplotlib:** Library for visualizing query performance results.
- **NumPy:** Used for numerical operations and data handling.

## Conclusion
This project serves as a comprehensive demonstration of data analysis capabilities in the e-commerce sector. By highlighting the impact of database indexing strategies on query performance, the findings provide valuable insights for data analysts and database administrators in optimizing query efficiency for real-world applications.
