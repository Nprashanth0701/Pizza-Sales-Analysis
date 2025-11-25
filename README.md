# 🍕 Pizza Sales Analysis

Uncovering insights from pizza sales data using SQL.

This project analyzes transactional pizza sales data and extracts meaningful business insights such as revenue, customer ordering behavior, product popularity, and category performance. The goal is to support data-driven decisions for menu design, promotions, and operations.

---

## 📊 Project Overview

The project explores a pizza business dataset using SQL to answer key questions:

- How many total orders were placed?
- What is the total revenue from pizza sales?
- Which is the highest-priced pizza?
- What is the most common pizza size ordered?
- Which pizza types are ordered the most?
- At what time of day do customers order the most?
- Which pizza category sells the most?
- What are the top pizzas by revenue?
- How much does each pizza category contribute to total revenue?
- How does revenue grow cumulatively over time?

Each question is solved using SQL queries and interpreted with business context.

---

## 📂 Dataset Structure

The dataset consists of four relational tables:

### `orders`
Contains high-level order information.
| Column | Description |
|------|-------------|
| order_id | Unique order identifier |
| order_date | Date of order |
| order_time | Time of order |

### `order_details`
Contains line items belonging to each order.
| Column | Description |
|------|-------------|
| order_details_id | Line item ID |
| order_id | Linked to orders table |
| pizza_id | Linked to pizzas table |
| quantity | Number of units ordered |

### `pizzas`
Contains product-level metadata.
| Column | Description |
|------|-------------|
| pizza_id | Unique pizza ID |
| pizza_type_id | Linked to pizza_types table |
| size | Pizza size (S, M, L, XL, XXL etc.) |
| price | Unit price |

### `pizza_types`
Contains catalog-level pizza information.
| Column | Description |
|------|-------------|
| pizza_type_id | Primary key |
| name | Pizza name |
| category | Category (Classic / Supreme / Chicken / Veggie) |
| ingredients | Ingredient list |

---

## 🔗 Data Model (ER Relationship)

