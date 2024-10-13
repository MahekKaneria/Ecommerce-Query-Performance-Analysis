# Index Optimization Report for Query Performance Analysis

**Prepared by:** Mahek Kaneria

## Project Overview

This project analyzes the performance of SQL queries by benchmarking different indexing strategies: uninformed, self-optimized, and user-optimized. It utilizes SQLite databases derived from a Kaggle dataset to evaluate how these strategies impact query execution times across three database sizes: small, medium, and large.

## Purpose of the Report

This report details the indices created for the “User Optimized” scenarios associated with the four queries analyzed in the project. The focus is on how these indices improve query performance through efficient data retrieval.

## Indices Created

For each of the four SQL queries analyzed, the following indices were implemented to optimize performance:

### 1. Index on `customer_postal_code` in the `Customers` Table
- **Purpose:** This index allows for quick filtering of customers based on their postal code.
- **Impact:** By reducing the number of records that need to be checked in the `Orders` table, this index significantly enhances query execution speed, leading to faster response times for queries that involve customer location filtering.

### 2. Index on `order_id` in the `Order_items` Table
- **Purpose:** This index facilitates faster access to orders containing multiple items, improving the subquery that checks for orders based on item count.
- **Impact:** The subquery groups records by `order_id` and checks their counts. Having an index on this column allows the database to perform these operations more efficiently, resulting in quicker aggregations and improved overall query performance.

## Performance Analysis

The implementation of the above indices allowed the queries to quickly filter and count the necessary records, leading to a marked improvement in performance. In real-world applications, such optimizations are crucial, as query execution time can significantly impact user experience and system efficiency.

## Conclusion

The analysis underscores the importance of database optimization through indexing strategies. By implementing targeted indices, the project successfully enhanced the performance of SQL queries, demonstrating strong data analysis capabilities and proficiency in SQL.
