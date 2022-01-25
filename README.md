# Amazon Vine Analysis

<https://github.com/skaram16/amazon_vine_analysis/blob/main/amazon.jpeg>

> Analyzing Amazon reviews written by members of the paid Amazon Vine program https://www.amazon.com/gp/vine/help.

## Objective

Like the majority of shoppers, Amazon's shoppers depend on product reviews to make a purchase decisions. Amazon makes their vine review datasets publicly available https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt. Vine reviews are quite large and can exceed the capacity of local machines to handle; hence, we are using Spark and AWS.

The first goal for this assignment will be to perform the ETL process completely in the cloud and upload a DataFrame to an RDS instance. The second goal will be to use PySpark to perform a statistical analysis of selected data.
