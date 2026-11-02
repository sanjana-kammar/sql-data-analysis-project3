# SQL Data Analysis – Project 3

**DecodeLabs | Data Analytics Internship | Batch 2026**

## Objective
Use SQL queries to extract business insights from an e-commerce orders dataset.

## Dataset
- 1,200 orders, Jan 2023 to Jun 2025
- Columns include Product, Quantity, UnitPrice, PaymentMethod, OrderStatus, CouponCode, ReferralSource and TotalPrice
- Cleaning: removed 3 empty stray columns; blank CouponCode values kept as NULL (no coupon used)

## Tools
SQLite (queries also work in MySQL, except `strftime`, which becomes `YEAR()`)

## SQL Concepts Used
SELECT, WHERE, ORDER BY, GROUP BY, HAVING, COUNT, SUM, AVG, aliases, subquery, COALESCE, strftime

## Files
| File | Description |
|------|-------------|
| `project3_sql_report.pdf` | 14 queries with outputs and insights |
| `project3_sql_queries.sql` | All SQL queries |
| `orders_clean.csv` | Cleaned dataset |
| `orders.db` | SQLite database (table: `orders`) |

## Key Findings
- About 41% of orders are cancelled or returned, the biggest revenue leak
- Printer and Chair contribute the most net revenue (about 16% each)
- Instagram is the strongest referral channel
- Credit Card orders have the highest average order value
- Coupons do not noticeably change order value, and repeat customers are rare

## How to Run
Open `orders.db` in DB Browser for SQLite and run the queries from `project3_sql_queries.sql`.

## Author
Sanjana
