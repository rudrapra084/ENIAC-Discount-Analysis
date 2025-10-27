# ENIAC-Discount-Analysis

## Overview
This project is a part of the **Data Science Bootcamp** at **WBS Coding School**.  
The analysis was conducted by **Surekha Jan**, **Aleksandra Dominika Gruszka**, and **Pranab Rudra**.  

The primary focus is on understanding how monthly revenue and the average discount rate influence sales performance during the years **2017 to 2018**.  
Additionally, the study explores the relationship between **discounts, seasonal shifts, special events, product categories**, and various **pricing and quantity dynamics**.

---

## Objective
To assess the impact of **Eniac's discounting strategy** on sales performance, categorization, and seasonal variations.  
The analysis aims to provide insights into optimizing discount distribution across product categories and months.

---

## Data Source
The data for this analysis is sourced from **Eniac's discount database**, covering the period from **2017 to 2018**.  
The dataset was cleaned to address issues such as a corrupted database, incongruent data, double-dot numbers, and general data quality concerns.

---

## Data Description
orders.csv – Every row in this file represents an order. order_id – a unique identifier for each order created_date – a timestamp for when the order was created total_paid – the total amount paid by the customer for this order, in euros state “Shopping basket” – products have been placed in the shopping basket “Place Order” – the order has been placed, but is awaiting shipment details “Pending” – the order is awaiting payment confirmation “Completed” – the order has been placed and paid, and the transaction is completed. “Cancelled” – the order has been cancelled and the payment returned to the customer.

orderlines.csv – Every row represents each one of the different products involved in an order. id – a unique identifier for each row in this file id_order – corresponds to orders.order_id product_id – an old identifier for each product, nowadays not in use product_quantity – how many units of that product were purchased on that order sku – stock keeping unit: a unique identifier for each product unit_price – the unitary price (in euros) of each product at the moment of placing that order date – timestamp for the processing of that product

products.csv sku – stock keeping unit: a unique identifier for each product name – product name desc – product description price – base price of the product, in euros promo_price – promotional price, in euros in_stock – whether or not the product was in stock at the moment of the data extraction type – a numerical code for product type

brands.csv short – the 3-character code by which the brand can be identified in the first 3 characters of products.sku long – brand name

---

## Tools Used
- **Python (Google Colab)** for data analysis  
- **Pandas** for data manipulation and cleaning  
- **Seaborn** for statistical visualization

---

## Data Cleaning
The dataset underwent a rigorous cleaning process to ensure data integrity:

1. **Corrupted Database:** Identified and addressed issues that affected the overall integrity of the database.  
2. **Incongruent Data:** Resolved inconsistencies, mismatched, and/or duplicate data.  
3. **Double-Dot Numbers:** Rectified anomalies in numerical values, focusing on duplicated or irregular decimal points.  
4. **Data Quality Concerns:** Mitigated issues affecting the reliability and completeness of the dataset.

---

## Analysis and Recommendations
Our analysis indicates that **higher discounts do not necessarily lead to higher revenue**.  
Eniac should therefore avoid blanket high-rate discounting strategies and focus instead on **strategic, time-limited offers**.

### Recommendations
1. Maintain discounts within a reasonable range to preserve margins.  
2. Improve data collection and extend observation periods to capture more seasonal trends.  
3. Ensure standardized product categorization and duplicate checks to refine future analyses.

---

**Date:** 27 October 2025  
**Authors:** Pranab Rudra, Surekha Jan, Aleksandra Dominika Gruszka 
