# Food Delivery Data Integration Project

This project demonstrates how to combine multiple real-world data sources into a single, analysis-ready dataset using Python. It simulates a typical data engineering workflow used in analytics and reporting systems.

## Data Files
- **orders.csv** – Transactional order data  
- **users.json** – User master data  
- **restaurants.sql** – Restaurant master data  

Each file is provided in a different format to reflect real production data scenarios.

## Objective
To merge all data sources into one final dataset that serves as the single source of truth for analysis.

## Process Overview
1. Load CSV data using Pandas  
2. Load and normalize JSON data  
3. Load SQL data using SQLite  
4. Merge datasets using left joins  
   - `orders.user_id` → `users.user_id`  
   - `orders.restaurant_id` → `restaurants.restaurant_id`

## Output
- **final_food_delivery_dataset.csv**

This dataset contains:
- Order details  
- User information  
- Restaurant information  

## Analysis Use Cases
- Order trends over time  
- User behavior patterns  
- City-wise and cuisine-wise performance  
- Membership impact (Gold vs Regular users)  
- Revenue distribution and seasonality  

## Tools and Technologies
- Python  
- Pandas  
- SQLite  
- Jupyter Notebook  

## How to Run
1. Install required libraries:
   ```bash
   pip install pandas
