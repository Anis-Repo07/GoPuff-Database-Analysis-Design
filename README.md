# GoPuff-Database-Analysis-Design
A scalable database system for GoPuff, built using Oracle APEX, to optimize order processing, inventory management, and delivery logistics.

## Background and Overview
GoPuff is an on-demand delivery service that provides customers with everyday essentials, snacks, drinks, and other products. Unlike traditional delivery platforms, GoPuff stocks thousands of products in micro-fulfillment centers to optimize delivery efficiency.
The goal of this project is to develop a scalable database system to efficiently manage GoPuff’s online ordering platform. This database will enable seamless order processing, inventory tracking, customer management, and delivery optimization, ensuring timely deliveries and accurate inventory management.
To achieve this, Oracle APEX was used as the primary database management tool for designing, querying, and optimizing the system. Oracle APEX provides a low-code environment that allows for rapid database application development, making it an ideal choice for structuring GoPuff’s backend operations.

## Data Structure Overview
### Entity-Relationship (ER) Model & Relational Schema:
The Entity-Relationship (ER) model is designed to reflect GoPuff’s core business operations, ensuring seamless order fulfillment, real-time inventory tracking, and efficient delivery routing.
Customers and Orders Relationship: Customers place multiple orders, and each order is linked to a specific customer through a foreign key relationship (CustomerID → Orders).

Order Processing & Product Catalog: Orders contain multiple products, requiring a many-to-many relationship handled through an intermediate table (OrderLine), ensuring accurate transaction tracking.

Inventory Management & Fulfillment Centers: Each product is stocked in different micro-fulfillment centers, enabling real-time stock level updates and supply chain optimization.

Delivery & Logistics: Orders are assigned to available drivers, and tracking is maintained via the Delivery table, ensuring efficient dispatch and customer notifications.

![image](https://github.com/user-attachments/assets/bf8970ad-a5dd-4848-aa3e-266ce2b70404)



The Relational Schema converts these business processes into a structured SQL-compatible format, implementing primary and foreign key constraints to enforce data integrity and streamline operational efficiency.
The ER model establishes relationships between customers, orders, products, and delivery hubs, ensuring a structured database framework.

The relational schema translates business processes into SQL-compatible tables with primary and foreign key constraints to maintain data integrity.

![image](https://github.com/user-attachments/assets/26521b2a-34d6-4da0-a40f-2735a2e3c6ff)


### Executive Summary
To ensure GoPuff’s operational efficiency, this project focuses on designing a robust, scalable database that optimizes key business processes.

Our database enables:

Efficient Customer & Order Management: Ensuring seamless order tracking and customer engagement.

Real-Time Inventory Management: Preventing stockouts and improving supply chain efficiency.

Optimized Delivery Routing: Assigning drivers and scheduling deliveries for faster service.

Vendor & Employee Management: Enhancing coordination with suppliers and workforce tracking.

By implementing a structured relational schema with optimized SQL queries, GoPuff can significantly improve order accuracy, delivery speed, and inventory management, driving higher customer satisfaction.

## Key Insights
The SQL queries implemented in this project provide deeper insights into GoPuff’s business operations by optimizing order management, tracking sales performance, and ensuring smooth inventory and delivery processes.

### Revenue Analysis:
What is the total revenue generated by each individual order?
- Querying total revenue generated by individual orders helps understand customer spending patterns and identify high-value transactions.
  paste the code snippet here

### Top-Selling Products:
What are the top-selling products?
- Analyzing sales by product category allows GoPuff to optimize inventory stocking and marketing strategies.

### Delivery & Driver Tracking:
What is the order history and total spending of a specific customer?
- Identifying active delivery drivers ensures efficient order fulfillment and route optimization.

## Recommendations
### For GoPuff’s Business Strategy:
Automate Inventory Replenishment: Implement automated restocking alerts based on real-time stock levels to prevent stockouts and reduce excess inventory.

Optimize Delivery Routing: Use AI-driven route optimization to assign orders dynamically, reducing delivery times and operational costs.

Improve Customer Personalization: Utilize customer order history data to offer personalized promotions and product recommendations.

Enhance Order Processing Efficiency: Streamline order-to-fulfillment workflows by integrating automated notifications and real-time updates for customers.
