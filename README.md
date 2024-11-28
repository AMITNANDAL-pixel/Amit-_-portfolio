# Amit-portfolio
Analytics portfolio

# Project 1 : Campaign/Discount OFFER  Effect On Revenue Increment/Sale Increment

## Project details
# Problem statement 
Analyze Promotions and Provide Tangible Insights to Sales Director

Domain: FMCG	Function: Sales / Promotions
AtliQ Mart is a retail giant having supermarkets in the southern region of India. All     their  stores ran a massive promotion during the Diwali 2023 and Sankranti 2024 (festive time in India) on their AtliQ branded products. Now the sales director wants to understand which promotions did well and which did not so that they can make informed decisions for their next promotional period.
we will analyze Different campaign effect on revenue increment and incremental sold quantity.

## Business Request/what business requirement
1.	Provide a list of products with a base price greater than 500 and that are featured in promo type of 'BOGOF' (Buy One Get One Free). This information will help us identify high-value products that are currently being heavily discounted, which can be useful for evaluating our pricing and promotion strategies.


2.	Generate a report that provides an overview of the number of stores in each city. The results will be sorted in descending order of store counts, allowing us to identify the cities with the highest store presence.The report includes two essential fields: city and store count, which will assist in optimizing our retail operations.


3.	Generate a report that displays each campaign along with the total revenue generated before and after the campaign? The report includes three key fields: campaign_name, total_revenue(before_promotion), total_revenue(after_promotion). This report should help in evaluating the financial impact of our promotional campaigns. (Display the values in millions)


4.	Produce a report that calculates the Incremental Sold Quantity (ISU%) for each category during the Diwali campaign.  The report will include  key fields: category, isu%. This information will assist in assessing the category-wise success and impact of the Diwali campaign on incremental sales.

Note: ISU% (Incremental Sold Quantity Percentage) is calculated as the percentage increase/decrease in quantity sold (after promo) compared to quantity sold (before promo)


5.	Create a report featuring the Top 5 products, ranked by Incremental Revenue Percentage (IR%), across all campaigns. The report will provide essential information including product name, category, and ir%. This analysis helps identify the most successful products in terms of incremental revenue across our campaigns, assisting in product optimization.


## Solution 
# 1.	Provide a list of products with a base price greater than 500 and that are featured in promo type of 'BOGOF' (Buy One Get One Free). This information will help us identify high-value products that are currently being heavily discounted, which can be useful for evaluating our pricing and promotion strategies.

create a measure 

premium product heavily discounted = FILTER(FACT_TABLE,FACT_TABLE[base_price]>500 && FACT_TABLE[promo_type]="BOGOF")




