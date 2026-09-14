# E-commerce Sales Funnel Analysis
E-commerce sales funnel analysis using SQL and Google BigQuery

## Project Overview

This project analyses customer behaviour across an e-commerce sales funnel using SQL and Google BigQuery.

The dataset contains over 9,000 customer event records covering page views, add-to-cart events, checkout activity, payment activity and purchases.

The objective was to understand where customers drop out of the funnel, compare the performance of different traffic sources and evaluate key revenue metrics.

## Tools Used

- SQL
- Google BigQuery
- GitHub

## Dataset

The dataset contains customer interaction events including:

- User ID
- Event type
- Event date
- Product ID
- Transaction amount
- Traffic source

Key funnel stages analysed:

1. Page View
2. Add to Cart
3. Checkout Start
4. Payment Information
5. Purchase

## Analysis Performed

### Sales Funnel Analysis

Measured the number of unique users reaching each stage of the customer journey and calculated conversion rates between stages.

### Traffic Source Analysis

Compared customer conversion across different acquisition channels to identify which traffic sources generated the strongest purchasing behaviour.

### Time-to-Conversion Analysis

Calculated the average time taken for customers to move from:

- Page view to add to cart
- Add to cart to purchase
- Page view to purchase

### Revenue Analysis

Calculated key commercial metrics including:

- Total revenue
- Total buyers
- Total orders
- Average order value
- Revenue per buyer
- Revenue per visitor

## SQL Techniques Used

- Common Table Expressions (CTEs)
- CASE statements
- Conditional aggregation
- COUNT DISTINCT
- GROUP BY
- HAVING
- SUM and AVG
- TIMESTAMP_DIFF
- Conversion-rate calculations

## Key Findings

Funnel Conversion
- 4,268 unique users viewed products, with 1,332 progressing to add-to-cart.
- View-to-cart conversion was approximately 31%.
- Around 71% of customers who added an item to their cart progressed to checkout.
- Checkout completion was strong, with approximately 92% of users reaching payment going on to purchase.

Funnel by Source
- The largest funnel drop-off occurred between product viewing and cart addition.
- The largest funnel drop-off occurred between page view and add-to-cart, indicating that converting initial product interest into purchase intent is the main area of opportunity.
- Email was the highest-converting traffic source, with a 62.45% view-to-cart rate and 33.91% purchase conversion rate, despite generating only 522 unique views.
- Social generated 1,472 unique views but had the weakest purchase conversion rate at just 6.93%, suggesting that high traffic volume did not translate into strong purchasing behaviour.
- Paid ads performed comparatively well, achieving a 21.07% purchase conversion rate, while organic traffic generated the highest overall volume with 2,038 unique views and 343 purchases.
- Once users added an item to their cart, conversion was relatively consistent across channels, with cart-to-purchase rates ranging from approximately 51% to 57%. This suggests that the biggest differences between traffic sources occur earlier in the customer journey.

## Recommendations

Based on the analysis:

- Investigate opportunities to improve the transition from product viewing to cart addition.
- Prioritise acquisition channels with stronger purchase conversion.
- Monitor customer acquisition cost alongside revenue per visitor and average order value.

## Files

- `ecommerce_funnel_analysis.sql` — SQL queries used for the analysis
- `user_events.csv` — source dataset
