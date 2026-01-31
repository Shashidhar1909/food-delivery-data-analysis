# 🍽 Food Delivery Data Integration & Analysis

## 📌 Project Overview
This project demonstrates an end-to-end data integration and analysis workflow
by combining data from multiple real-world formats into a single analytical dataset.

The goal is to create a **single source of truth** for analyzing user behavior,
order trends, revenue distribution, and membership impact in a food delivery system.

---

## 📂 Data Sources
The project uses three different datasets, each representing a real-world system:

- **orders.csv** – Transactional order-level data  
- **users.json** – User master data  
- **restaurants.sql** – Restaurant master data (stored in SQL format)

---

## 🔗 Data Integration Logic
The datasets are combined using the following keys:

- `orders.user_id` → `users.user_id`
- `orders.restaurant_id` → `restaurants.restaurant_id`

**Join Type:** LEFT JOIN  
This ensures all orders are retained even if corresponding user or restaurant
details are missing.

---

## 📁 Final Output
- **final_food_delivery_dataset.csv**

This dataset contains:
- Order details
- User information
- Restaurant information

It acts as the **only source of truth** for all analysis and questions.

---

## 📊 Analysis & Insights
Using the final dataset, the following analyses are performed:

- Order trends over time
- User behavior patterns
- City-wise and cuisine-wise performance
- Gold vs Regular membership impact
- Revenue distribution and seasonality

---

## 🛠 Tech Stack
- Python
- Pandas
- SQLite
- Jupyter Notebook

---

## 🚀 How to Run the Project
1. Clone the repository
2. Install dependencies  
