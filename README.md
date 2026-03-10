# Oldest Businesses in the World - SQL Analysis

## Overview
This project explores the oldest functioning businesses across the globe, investigating the unique characteristics and industries that enable a business to stand the test of time. Inspired by data sourced from BusinessFinancing.co.uk, this SQL-driven analysis combines multiple datasets to uncover historical insights into global commerce dating back as far as the year 578.

## The Dataset
The dataset relies on several relational tables containing data about historically significant businesses, their categories, and their geographic locations:
- 🏢 **`businesses` & `new_businesses`**: Contains the name of the business, the year it was founded, its category code, and its country code.
- 🌍 **`countries`**: Maps three-letter country codes to the actual country name and its continent.
- 🏷️ **`categories`**: Maps category codes to detailed descriptions of the business category (e.g., Agriculture, Banking & Finance, Aviation & Transport).

## Key Questions Answered
The analysis comprehensively answers the following questions using SQL joins, subqueries, and aggregations:
1. **What is the oldest business on each continent?** (e.g., Kongō Gumi in Asia founded in 578, St. Peter Stifts Kulinarium in Europe founded in 803).
2. **How many countries per continent lack data on the oldest businesses?** (Evaluated by performing `LEFT JOIN`s and exploring the effect of incorporating `new_businesses` data).
3. **Which business categories are best suited to last over the course of centuries?** (Determined by grouping the minimum founding year across continents and specific business categories).

## Repository Contents
- `notebook.ipynb`: The core Jupyter Notebook containing the interactive SQL data analysis and results.
- `MKn_Staffelter_Hof.jpeg`: An image of Staffelter Hof Winery (Germany's oldest business, established in 862), used to present historical context in the project notebook.

## Technologies Used
- **SQL (PostgreSQL)**: For extensive data manipulation, grouping, and multi-table joins.
- **Jupyter Notebook**: For interactive data querying, formatted output presentation, and documentation.
