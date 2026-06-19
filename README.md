# 🛒 Customer Shopping Behavior Analysis

## 📌 Overview
This project explores customer shopping behavior to uncover insights around purchasing patterns, subscription impact, discount effectiveness, and customer segmentation. The analysis follows a full data analytics pipeline — from data loading and cleaning in Python, to SQL querying on PostgreSQL, to building an interactive Tableau dashboard.

---

## 📂 Dataset
- **File:** `customer_shopping_behavior.csv`

| Column | Description |
|---|---|
| `customer_id` | Unique identifier for each customer |
| `gender` | Male or Female |
| `age_group` | Customer age segment |
| `category` | Product category |
| `item_purchased` | Specific item bought |
| `purchase_amount` | Transaction amount (USD) |
| `review_rating` | Customer review score |
| `subscription_status` | Subscribed or Not Subscribed |
| `discount_applied` | Whether a discount was used (Yes/No) |
| `shipping_type` | Standard, Express, etc. |
| `previous_purchases` | Number of prior purchases |

---

## 🛠 Tools & Technologies

| Tool | Purpose |
|---|---|
| **Python (Pandas)** | Data loading, cleaning, and EDA |
| **PostgreSQL** | Database storage and SQL analysis |
| **pgAdmin 4** | PostgreSQL GUI management |
| **Tableau** | Interactive dashboard and visualizations |

---

## 🔍 Analysis Steps

### 1. Data Loading & Cleaning (Python)
- Loaded the CSV dataset using Pandas
- Handled missing values and duplicates
- Standardized data types and column formatting

### 2. SQL Analysis (PostgreSQL)
Loaded the cleaned data into PostgreSQL and wrote queries to answer key business questions:

- **Q1.** Total revenue by gender
- **Q2.** Customers who used discounts but still spent above average
- **Q3.** Top 5 products by average review rating
- **Q4.** Average purchase amount: Standard vs. Express shipping
- **Q5.** Revenue and spending comparison: Subscribers vs. Non-Subscribers
- **Q6.** Top 5 products with the highest discount usage rate
- **Q7.** Customer segmentation into New, Returning, and Loyal based on purchase history
- **Q8.** Top 3 most purchased products within each category
- **Q9.** Are repeat buyers more likely to subscribe?
- **Q10.** Revenue contribution by age group

### 3. Dashboard (Tableau)
Built an interactive Tableau dashboard featuring:
- KPI cards for key metrics (total customers, revenue, etc.)
- Donut chart for subscription status breakdown
- Bar charts for revenue by category and age group
- Filters for dynamic exploration

---

## 📊 Dashboard Preview

<img width="1275" height="800" alt="image" src="https://github.com/user-attachments/assets/ad573a28-b876-4922-8bd4-a07a1c78dcee" />

---

## 📈 Key Insights
- **Male customers generate more total revenue** than female customers
- **Non-subscribers spend more** than subscribers, suggesting subscription status does not drive higher spending
- **Top 5 highest-rated products** by average review rating: Gloves, Sandals, Boots, Hat, and Skirt
- **Repeat buyers are less likely to subscribe**, indicating that loyal customers may not see enough value in the subscription model
- **Young adults are the largest revenue contributors**, making them a key demographic for targeted marketing

---

## 📁 Project Structure
```
customer_behavior_analysis/
│
├── Customer_Shopping_Behavior_Analysis.ipynb   # Python EDA notebook
├── customer_shopping_behavior.csv              # Raw dataset
├── customer_behavior.sql                       # SQL queries
├── customer_behavior.twbx                      # Tableau dashboard
└── README.md                                   # Project documentation
```
