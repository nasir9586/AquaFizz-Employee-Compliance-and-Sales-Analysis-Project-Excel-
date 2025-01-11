# AquaFizz-Employee-Compliance-and-Sales-Analysis-Project-Excel-
Employee Working Hours and Customer Order Analysis

**Project Overview**

**Objective**
The main goal of this project is to analyze employee working hours and customer order data to ensure compliance with AquaFizz’s policies and optimize sales. The analysis involves examining data on working hours for compliance and generating business insights from customer and sales data.

Company Background:
AquaFizz is a newly established beverage startup offering health-focused sparkling water beverages. The company aims to provide refreshing, nutrient-enhanced drinks while promoting overall wellness.

**Business Task**
Analyzing employee working hours for compliance with the company's standards.
Analyzing sales data to gain insights into customer behavior and identify top-performing products.
Data Understanding
Employee Working Hours Data

Dataset Name: Workers Timing Dataset
Dataset Includes:
Time of entry: Timestamp of when employees clocked in.
Time of exit: Timestamp of when employees clocked out.

Orders Data
Dataset Name: Orders Dataset
Dataset Includes:
date: Date the order was placed.
order_id: Unique identifier for each order.
customer_id: Identifier linking the order to a customer.
beverage: The type of beverage ordered.
cost_price: The cost price of the beverage.
selling_price: The price at which the beverage was sold.

Customers Data
Dataset Name: Customer Dataset
Dataset Includes:
customer_id: Unique identifier for each customer.
first_name: Customer’s first name.
last_name: Customer’s last name.
email: Customer’s email address.
city: The city where the customer is located.
country: The country of residence for the customer.
user: User type identifier.
code: Customer code for internal use.

Data Preprocessing
Employee Working Hours Data Processing:
Convert Working Time to Decimal:
Convert the benchmark working time (8 hours and 30 minutes) into decimal format (8.5 hours).
Calculate Actual Working Hours:
Convert minutes worked into fractions of an hour (e.g., 30 minutes = 0.5 hours) and sum them with whole hours worked.
Determine Compliance:
Compare actual working hours with the benchmark (8.5 hours) with a tolerance of ±6 minutes.

Hours and Minutes Worked Calculation:
Break down the total hours worked into whole hours and minutes for clear visualization.

Deviation in Minutes:
For non-compliant entries, calculate the deviation in minutes compared to the benchmark time.

Non-Compliance Message:
Generate a message for non-compliant cases with specific details about the date, hours worked, and deviation.

Orders and Customers Data Processing:
Profit Calculation:
Calculate profit per sale as the difference between selling_price and cost_price for each order in the Orders dataset.

Top 5 Customers by Sales:
Aggregate sales by customer_id and identify the top 5 customers with the highest total sales.

Top Cities by Sales:
Aggregate sales by city (from the Customers dataset) and identify the top-performing cities contributing the most to sales.

Monthly Sales Analysis:
Extract the month from the order date and calculate the total profit for each month. Create a chart to visualize monthly sales trends.

Highest Profit % Beverage:
Calculate the profit margin for each beverage — ((Selling Price - Cost Price) / Cost Price) — and identify the beverage with the highest profit margin.

Top 10 Beverage Purchasers:
Identify the top 10 customers who purchased the most beverages based on the total number of orders.

Excel Dashboard Creation:
Combine results into a comprehensive Excel dashboard for easy visualization of key insights.

**Business Value**
This project provided actionable insights to AquaFizz for optimizing employee performance and improving customer sales strategies. By analyzing working hours and sales data, the company can ensure compliance, boost efficiency, and increase profitability.
