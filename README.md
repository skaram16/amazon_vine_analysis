# Amazon Vine Analysis

<img src='https://github.com/skaram16/amazon_vine_analysis/blob/main/amazon.jpeg'>


Since your work with Jennifer on the SellBy project was so successful, you’ve been tasked with another, larger project: analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

In this project, you’ll have access to approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. You’ll need to pick one of these datasets and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, you’ll use PySpark, Pandas, or SQL to determine if there is any bias toward favorable reviews from Vine members in your dataset. Then, you’ll write a summary of the analysis for Jennifer to submit to the SellBy stakeholders.


> Analyzing Amazon reviews written by members of the paid Amazon Vine program https://www.amazon.com/gp/vine/help.

## Objective

Like the majority of shoppers, Amazon's shoppers depend on product reviews to make a purchase decisions. Amazon makes their vine review datasets publicly available https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt. Vine reviews are quite large and can exceed the capacity of local machines to handle; hence, we are using Spark and AWS.

The first goal for this assignment will be to perform the ETL process completely in the cloud and upload a DataFrame to an RDS instance. The second goal will be to use PySpark to perform a statistical analysis of selected data.

### Data

DATA COLUMNS:
marketplace - 2 letter country code of the marketplace where the review was written.
customer_id - Random identifier that can be used to aggregate reviews written by a single author.
review_id - The unique ID of the review.
product_id - The unique Product ID the review pertains to. In the multilingual dataset the reviews
for the same product in different countries can be grouped by the same product_id.
product_parent - Random identifier that can be used to aggregate reviews for the same product.
product_title - Title of the product.
product_category - Broad product category that can be used to group reviews
(also used to group the dataset into coherent parts).
star_rating - The 1-5 star rating of the review.
helpful_votes - Number of helpful votes.
total_votes - Number of total votes the review received.
vine - Review was written as part of the Vine program.
verified_purchase - The review is on a verified purchase.
review_headline - The title of the review.
review_body - The review text.
review_date - The date the review was written.
