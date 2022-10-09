# Amazon_Vine_Analysis

##   Overview of the analysis of the Vine program:

This project is about Amazon Vine Program, a service that allows manufacturers and publishers to receive reviews for their products. The purpose of this project is to analyze reviews written by members of the paid Amazon Vine program.

A dataset has been selected from [Amazon Review Datasets](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt)

selected data: https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Apparel_v1_00.tsv.gz

Using PySpark, we performed the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin.

## Results:

Total Paid Vine Reviews: **33**
![Vines Reviews](https://raw.githubusercontent.com/Mishabatoon/Amazon_Vine_Analysis/main/screenshots/Number%20of%20Vine%20Reviews.png)

Total Non-Vine Reviews: **45,388**
![enter image description here](https://raw.githubusercontent.com/Mishabatoon/Amazon_Vine_Analysis/main/screenshots/Non-vine%20reviews.png)

Total Paid Vine 5-star Rating: **15**
![Paid5star](https://raw.githubusercontent.com/Mishabatoon/Amazon_Vine_Analysis/main/screenshots/Paid%205_Star%20rating.png)

Total Unpaid Vine 5-star Rating: **23,733**
![unpaid5star](https://raw.githubusercontent.com/Mishabatoon/Amazon_Vine_Analysis/main/screenshots/Unpaid%205%20star%20rating.png)



## Summary:

Out of 33 Vine reviews, only 15 were 5-star ratings which is only 45.45% success rate. The success rate of 5-star reviews from non-vine program is 52.29% which is higher than the vine reviews. Thus, there is no bias toward favorable reviews from Vine members in the dataset.

Additionally, we can run a T-test to calculate if there is a significant difference between the means of two groups (Vine vs Non-Vine).
