# Index Optimization Report for Query Performance Analysis

**Prepared by:** Mahek Kaneria

## Project Overview

This project aims to analyze the performance of SQL queries by benchmarking different indexing strategies: uninformed, self-optimized, and user-optimized. It utilizes SQLite databases derived from a Kaggle dataset to evaluate how these strategies impact query execution times across three database sizes: small, medium, and large.

## Purpose of the Report

This report details the indices created for the “User Optimized” scenarios associated with the four queries analyzed in the project. The focus is on how these indices improve query performance through efficient data retrieval.

## Indices Created

For each of the four SQL queries analyzed, the following indices were implemented to optimize performance:

### 1. Index on `customer_postal_code` in the `Customers` Table:
- **Purpose:** This index allows for quick filtering of customers based on their postal code.
- **Impact:** By reducing the number of records that need to be checked in the `Orders` table, this index significantly enhances query execution speed.

### 2. Index on `order_id` in the `Order_items` Table:
- **Purpose:** This index facilitates faster access to orders with multiple items by speeding up the subquery that checks for orders based on item count.
- **Impact:** Since the subquery groups records by `order_id` and checks their counts, having an index on this column allows the database to perform these operations more efficiently.

## Performance Analysis

With the implementation of the above indices, the queries were able to quickly filter and count the necessary records, leading to a marked improvement in performance. The use of these indices is crucial in real-world applications where query execution time can significantly affect user experience and system efficiency.

## Conclusion

The analysis demonstrates the importance of database optimization through indexing strategies. By implementing targeted indices, the project successfully improved the performance of SQL queries, showcasing strong data analysis capabilities and proficiency in SQL.
