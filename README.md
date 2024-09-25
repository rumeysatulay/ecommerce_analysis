# E-commerce Data Analysis

## Overview
In this project, I used a dataset from the Advanced SQL: MySQL for E-commerce Data Analysis course. With various data from an e-commerce company, I gained valuable insights.

## Dataset
This dataset comes from a Udemy course, *[Advanced SQL: MySQL for E-commerce Data Analysis](https://www.udemy.com/course/advanced-sql-mysql-for-analytics-business-intelligence/)*. There are 6 tables in the dataset. The tables and their columns are as follows:

1. **order_item_refunds**: `order_item_refund_id`, `created_at`, `order_item_id`, `order_id`, `refund_amount_usd`
2. **order_items**: `order_item_id`, `created_at`, `order_id`, `product_id`, `is_primary_item`, `price_usd`, `cogs_usd`
3. **orders**: `order_id`, `created_at`, `website_session_id`, `user_id`, `primary_product_id`, `items_purchased`, `price_usd`, `cogs_usd`
4. **products**: `product_id`, `created_at`, `product_name`
5. **website_pageviews**: `website_pageview_id`, `created_at`, `website_session_id`, `pageview_url`

## Project Goals
In this project, I examined website sessions, the conversion rates from sessions to orders, the stages at which customers drop off during the ordering process, product analysis, and user behavior analysis. The goal was to better understand how to increase profits. As a result, there are several important insights regarding the e-commerce company's performance.

## Process
SQL was the cornerstone of my analysis, enabling me to thoroughly examine the data and uncover crucial insights. I used Power BI for visualizing the data.

## Outcomes

- When we examine the website session data, it is evident that the gsearch utm_source appears to be the biggest driver of the business. Let's analyze the monthly trends for gsearch sessions and orders to assess growth. Using SQL, we extracted the total number of website sessions and orders by year and month. Using this data, we calculated the conversion rate of sessions to orders. Below, you can see the table and graph related to this analysis. While there is a significant increase in the number of sessions, the increase in the number of orders is much less pronounced. However, the overall conversion rate has also increased over time.

![2](https://github.com/user-attachments/assets/c3d629be-2a24-48b2-a246-dfb8f46092b7) ![1](https://github.com/user-attachments/assets/b8629d43-ca22-488d-992c-52e8166fcaf5)

- Now I wonder what would happen if I split this analysis into brand and non-brand categories for gsearch. It would be insightful to see whether brand searches are increasing. Brand campaigns represent users who explicitly search for your business in search engines. Therefore, an increase in the conversion rate of brand campaigns is a positive sign for the company and an important improvement to highlight to investors

![3](https://github.com/user-attachments/assets/0082133d-1a6c-4aa6-b6dc-5bc575ebe74a)


