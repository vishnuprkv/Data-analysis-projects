## Project Overview

To analyze Apple’s global sales data to uncover product performance trends, regional disparities, and operational inefficiencies, supporting data-driven business decisions.

## Entity Relationship Diagram (ERD)

![ERD](https://github.com/vishnuprkv/applesalesanalysis/blob/main/erd.png)

---

## Database Schema

The project uses five main tables:

1. **stores**: Contains information about Apple retail stores.
   - `store_id`: Unique identifier for each store.
   - `store_name`: Name of the store.
   - `city`: City where the store is located.
   - `country`: Country of the store.

2. **category**: Holds product category information.
   - `category_id`: Unique identifier for each product category.
   - `category_name`: Name of the category.

3. **products**: Details about Apple products.
   - `product_id`: Unique identifier for each product.
   - `product_name`: Name of the product.
   - `category_id`: References the category table.
   - `launch_date`: Date when the product was launched.
   - `price`: Price of the product.

4. **sales**: Stores sales transactions.
   - `sale_id`: Unique identifier for each sale.
   - `sale_date`: Date of the sale.
   - `store_id`: References the store table.
   - `product_id`: References the product table.
   - `quantity`: Number of units sold.

5. **warranty**: Contains information about warranty claims.
   - `claim_id`: Unique identifier for each warranty claim.
   - `claim_date`: Date the claim was made.
   - `sale_id`: References the sales table.
   - `repair_status`: Status of the warranty claim (e.g., Paid Repaired, Warranty Void).

## Business Questions

1. Find the number of stores in each country.
2. Calculate the total number of units sold by each store.
3. Identify how many sales occurred in December 2023.
4. Determine how many stores have never had a warranty claim filed.
5. Calculate the percentage of warranty claims marked as "Warranty Void".
6. Identify which store had the highest total units sold in the last year.
7. Count the number of unique products sold in the last year.
8. Find the average price of products in each category.
9. How many warranty claims were filed in 2020?
10. For each store, identify the best-selling day based on highest quantity sold.
11. Identify the least selling product in each country for each year based on total units sold.
12. Calculate how many warranty claims were filed within 180 days of a product sale.
13. Determine how many warranty claims were filed for products launched in the last two years.
14. List the months in the last three years where sales exceeded 5,000 units in the USA.
15. Identify the product category with the most warranty claims filed in the last two years.
16. Determine the percentage chance of receiving warranty claims after each purchase for each country.
17. Analyze the year-by-year growth ratio for each store.
18. Calculate the correlation between product price and warranty claims for products sold in the last five years, segmented by price range.
19. Identify the store with the highest percentage of "Paid Repaired" claims relative to total claims filed.
20. Write a query to calculate the monthly running total of sales for each store over the past four years and compare trends during this period.


## Project Focus

Utilize SQL functions like aggregations, joins, window functions, and time-based analysis to derive business insights on sales and warranty claims.

## Dataset

- **Size**: 1 million+ rows of sales data.
- **Period Covered**: The data spans multiple years, allowing for long-term trend analysis.
- **Geographical Coverage**: Sales data from Apple stores across various countries.

## Conclusion

Analyzed sales trends and warranty claims for different regions and products, providing insights that will help to improve product quality, after-sales service, and business focus in weak markets. The insights will support the company in refining warranty policies, addressing key problem areas, and enhancing customer satisfaction.
---
