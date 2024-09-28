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
  
![2](https://github.com/user-attachments/assets/ceb8140a-c2dc-4d48-8c27-e36ba49c5ce2)
![1](https://github.com/user-attachments/assets/6f78f360-fd32-4877-b842-48c104c9e9b8)


- Now I wonder what would happen if I split this analysis into brand and non-brand categories for gsearch. It would be insightful to see whether brand searches are increasing. Brand campaigns represent users who explicitly search for your business in search engines. Therefore, an increase in the conversion rate of brand campaigns is a positive sign for the company and an important improvement to highlight to investors

![3](https://github.com/user-attachments/assets/01c42f64-6cbe-4d46-b361-f23f4eb028c8)


- Now let's compare the session-to-order conversion rate between mobile and desktop devices. This analysis provides insight into which improvements should be made based on device type. As seen in the table, the conversion rate on desktop is higher, and the increase in conversion rate is also greater for desktop devices compared to mobile. Therefore, if any improvements are to be made, the focus should be on enhancing the desktop user interface, as customers are more likely to place orders from desktop devices.

![4](https://github.com/user-attachments/assets/3ddcce45-6c67-4168-87c4-8dd1fff2f700)

- I analyzed two landing pages (home and lander-1) to show the full conversion funnel from each of these pages to orders. To do this, I focused on the period starting from the launch of the lander page and the following month. I tracked every website session that started with either the home or lander page and followed the corresponding website pageviews for each session. The analysis focused on one product: MrFuzzy. As shown in the graph, the lander page’s conversion rate to orders is as good as the home page’s. Therefore, we can conclude that creating and improving the lander page leads to better outcomes and an increased order rate.

![5](https://github.com/user-attachments/assets/67433887-87b2-42e0-a3c8-e80f10c5fc68)

- Now let's examine the changes in revenue per order and per session over the years to assess overall business growth. To do this, we extracted the number of sessions, orders, and product prices by year. This allows us to calculate the revenue per order and per session. As shown in the table, the average revenue per order has increased from $49.99 to $62.80 over the past three years. This suggests that customers are likely buying more products over time, assuming product prices remain constant. Additionally, revenue per session has tripled in the same period. This indicates that, over the years, customers who visit the website are increasingly likely to make purchases. This growth is significant and should be shared with stakeholders.

![6](https://github.com/user-attachments/assets/dfa6d2f2-d0d8-474e-81e7-8f340c95aa82)

- Now it's time to examine which channel has experienced the most growth. We have non-brand gsearch, bsearch, organic search orders, and direct search orders. In this analysis, we considered the average orders for each quarter of each year, since the data for 2015 is incomplete, allowing for a fair comparison. As seen in the table, the largest portion of orders comes from the non-brand gsearch channel. Therefore, the majority of improvements and budget should be allocated to this channel. However, it's also important to note that organic and direct search orders have significantly increased over the years, which is a clear sign of success and growth in the business

![7](https://github.com/user-attachments/assets/d5f42c26-e7ec-41ba-a6e2-1c6cd8b1495c)

- Now let's examine seasonality, which refers to changes in sales throughout the year. For this analysis, I classified monthly revenue over a span of three years. To do this, I grouped the sales data by month and calculated the average revenue for each. As we can see, both revenue and sales tend to decrease during the summer months, while average revenue nearly doubles in the winter. Therefore, we can conclude that cooler weather encourages customers to purchase these products more frequently

![7](https://github.com/user-attachments/assets/22bf6e68-f3b8-4494-a338-a42b84667dbd)

- I also analyzed which product contributes the most to total revenue. As shown in the pie chart, the largest portion of revenue comes from Mr. Fuzzy with 60%, followed by Love Bear and Sugar Panda with 17% and 15%, respectively. The smallest portion, 8%, belongs to Mini Bear. This order is expected since Mr. Fuzzy has the highest sales volume.

![9](https://github.com/user-attachments/assets/f29874ea-1c3c-4fb4-8373-d38faf37a20d)

- Lastly, let's take a look at cross-selling. This analysis helps us understand if customers who buy a specific product are more likely to purchase another specific product. It also guides us in tailoring advertising strategies for each customer. Based on the table, we can see that customers who buy products 1, 2, and 3 tend to also purchase product 4. However, customers who primarily purchase product 4 are less likely to buy a second product.

![10](https://github.com/user-attachments/assets/139801ba-885f-44ce-9919-5863d603fa7d)


