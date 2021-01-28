# Amazon_Vine_Analysis

## Project Overview
To analyze 50 datasets of reviews written by members of the paid Amazon vine program and determine if there was a bias present. Amazon Vine is a service allowing manufacturers to collect reviews for their products. To determine bias we followed these steps:

- Picked a dataset to extract, transform and load the data to pgAdmin.
- Connected to an AWS RDS instance.
- Used PySpark to determine bias by creating dataframes to organize and isolate the information. 

## Resources
- Data Source: https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt
- Software: Google Collab, PySpark, PostgreSQL 4. 

## Results 
I chose to survey a dataset consisting of information about jewelry sales. 
![Vine Table DF](https://user-images.githubusercontent.com/71476009/106196631-46b1ec00-6177-11eb-9690-c460cb1e4dde.png)

- There were 7,689 non Vine reviews, and 21 Vine reviews. 
- There were 11 5-star Vine reviews, and 4444 non Vine 5-star reviews. 
- 53% percent of Vine reviews were 5-star.
- 57% precent of non Vine reviews were 5-star. 


## Summary

