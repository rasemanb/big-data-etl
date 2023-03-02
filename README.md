# big-data-etl

# Background

In this assignment, you will put your ETL skills to the test. Many of Amazon's shoppers depend on product
reviews to make a purchase. Amazon makes these datasets publicly available. They are quite large and can
exceed the capacity of local machines. One dataset alone contains over 1.5 million rows; with over 40
datasets, data analysis can be very demanding on the average local computer. Your first goal will be to
perform the ETL process completely in the cloud and upload a DataFrame to an RDS instance. The second goal
will be to use PySpark or SQL to perform a statistical analysis of selected data.

   - Part 1: Extract two Amazon customer review datasets, transform each dataset into four DataFrames, and   load the DataFrames into an RDS instance.

# Extract 

1. Read in each dataset using the correct header and sep parameters.
2. Get the number of rows in the dataset.

# Transform

1. Create the "review_id_df" DataFrame with the appropriate columns and data types.
2. Create the "products_df" DataFrame that drops the duplicates in the "product_id" and "product_title columns.
3. Create the "customers_df" DataFrame that groups the data on the "customer_id" by the number of times a customer reviewed a product.
4. Create the "vine_df" DataFrame that has the "review_id", "star_rating", "helpful_votes", "total_votes", and "vine" columns.

# Load

Export each DataFrame into the RDS instance to create four tables for each dataset.
