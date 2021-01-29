# Amazon_Vine_Analysis

## Project Overview
To analyze 50 datasets of reviews written by members of the paid Amazon vine program and determine if there was a bias present. Amazon Vine is a service allowing manufacturers to collect reviews for their products. To determine bias we followed these steps:

- Picked a dataset to extract, transform and load the data to pgAdmin.
- Connected to an AWS RDS instance.
- Used PySpark to determine bias by creating dataframes to organize and isolate the information. 

## Resources
- Data Source: https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt, https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Jewelry_v1_00.tsv.gz
- Software: Google Collab, PySpark, PostgreSQL 11, PgAdmin 4. 

## Results 
I chose to survey a dataset consisting of information about jewelry sales. 
![Vine Table DF](https://user-images.githubusercontent.com/71476009/106196631-46b1ec00-6177-11eb-9690-c460cb1e4dde.png)

Created a filtered dataframe where the total votes were equal or were greater than 20. 
![Total Votes Equal or Greater Than 20](https://user-images.githubusercontent.com/71476009/106198791-19b30880-617a-11eb-8e38-c7841cfc5f3a.png)

Created a filtered dataframe where helpful votes divided by total votes were equal or greater than 50%. 
![Greater than or equal to 50](https://user-images.githubusercontent.com/71476009/106199030-6f87b080-617a-11eb-9561-9727685e4f53.png)

Created a filtered dataframe with Vine (paid) reviews included. 
![Vine Reviews](https://user-images.githubusercontent.com/71476009/106199210-bc6b8700-617a-11eb-9c23-8ac067b1e7f1.png)

Created a filtered dataframe with non Vine (unpaid) reviews included. 
![Screen Shot 2021-01-28 at 3 09 17 PM](https://user-images.githubusercontent.com/71476009/106199269-cf7e5700-617a-11eb-867b-aeae88d0eb25.png)

- There were 7,689 non Vine reviews, and 21 Vine reviews. 
- There were 11 5-star Vine reviews, and 4444 non Vine 5-star reviews. 
- 53% percent of Vine reviews were 5-star.
- 57% precent of non Vine reviews were 5-star. 


## Summary
There doesn't appear to be a bias from the paid Vine reviews. The percentage of 5-star Vine reviews at 53% is pretty even with non Vine reviews at 57%. The main note is there is a significant difference in the amount of reviews. To get a more accurate reading, I would suggest surveying the 4 and 3-star Vine (paid) ratings. 

