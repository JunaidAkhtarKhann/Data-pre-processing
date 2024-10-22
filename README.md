In this Olist e-commerce project, the data model created in Power BI integrates multiple datasets to analyze customer orders and performance. Here's a breakdown of the relationships shown in the model:

Customers Dataset: This table contains customer information such as city, state, and postal code, with a unique customer_id. It is related to the Orders Dataset via the customer_id, allowing insights into customer orders.

Sellers Dataset: Holds seller information (city, state, etc.) and is linked to the Orders Dataset by the seller_id, providing the ability to analyze orders by seller locations and performance.

Orders Dataset: Central to the model, this fact table includes fields like order_id, price, freight_value, and customer_id, connecting various entities such as customers, sellers, and products. It acts as a hub between the other datasets.

Products Dataset: Contains product-related information (category, dimensions, etc.), linked to the Orders Dataset through product_id, helping in analyzing sales across different product categories.

Payment Mode Dataset: Includes details about payment types and installments for each order_id, connected to the Orders Dataset via order_id, offering insights into payment trends.

Delivery Status Dataset: Captures information about delivery statuses like delivery dates and customer expectations. Linked to the Orders Dataset, it helps analyze delivery performance.

Reviews Dataset: Provides customer reviews and scores, connected to order_id, allowing a correlation of product reviews with sales and delivery.

Date Table: A typical date dimension, connected to order and review dates, enabling time-based analysis such as sales trends and delivery timelines.

In summary, this model allows for comprehensive analysis of customer orders, product performance, payment modes, delivery statuses, and customer feedback, ensuring a holistic view of the e-commerce operations.
