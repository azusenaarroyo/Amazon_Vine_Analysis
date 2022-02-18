# Amazon Vine Analysis

## Overview of Analysis
The purpose of this analysis is to determine if there is any bias toward favorable reviews from Vine members in Amazon's Vine Program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products from Amazon Vine members, who are required to publish a review. The following analysis is of a video game dataset. The analysis uses PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. 

## Results

* In total, there are 4,291 Vine reviews, and 40,471 non-Vine reviews.
* Of the 4,291 Vine reviews, 1,607 are 5 star reviews or 37.45%.
* Of the 40,471 non-Vine reviews, 15,663 are 5 star reviews or 38.70% 

<img width="756" alt="vine_analysis_reviews" src="https://user-images.githubusercontent.com/91927712/154615593-2e7d861a-ccd5-47b6-b5f3-ff6f50e0ea52.png">

## Summary
In conclusion, there doesn't seem to be a positivity bias for reviews in the Vine program because the percentage of reviews from paid Vine and unpaid reviews are within 2% of each other. I would recommend filtering 4 star reviews by Vine member and unpaid reviews to determine if there is a positivity bias in 4 star ratings.
