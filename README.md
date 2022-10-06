# "Alexa, can You Handle Big Data?"
#### Created by: Estela Perez


## Objective 
The purpose of this assignment was to use cloud ETL skills on big data from two of Amazon's available public datasets on product reviews. The goal is to perfrom the ETL process completely in the cloud and upload a DataFrame to an RDS instance.

This project required the use of Amazon Web Service (AWS), Relational Database Service (RDS), pgAdmin, google Colab, PySpark, and Google Colab

## AWS-RDS
Started by creating an AWS-RDS to connect to pgAdmin
![alt text](level-1/images/AWS_RDS.png)

## pgAdmin
Then registered our AWS-RDS server in pgAdmin - displaying our databases for both datasets

![alt text](level-1/images/server_pgadmin.png)

## ETL Process: Pet Products Dataset
### Extract
* Extracted dataset:  https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Pet_Products_v1_00.tsv.gz
* Extracted number or records: 2,643,619 

![image](https://user-images.githubusercontent.com/98370960/191393863-4b6d4d43-ec24-4723-b8ab-a59d0747416b.png)


### Transform
![image](https://user-images.githubusercontent.com/98370960/191392900-4f54c3d0-aa8b-450c-adf7-fa0580ae42a2.png)
![image](https://user-images.githubusercontent.com/98370960/191392771-39df5312-d6bd-44f3-add0-15a9295750a8.png)
![image](https://user-images.githubusercontent.com/98370960/191393415-93c7007d-373b-4c0b-9e95-003ada6a0ab8.png)
![image](https://user-images.githubusercontent.com/98370960/191393582-ff94a746-e55d-4d85-8562-f4fb1b451a23.png)
![image](https://user-images.githubusercontent.com/98370960/191393668-88170edf-5d66-4db9-a6ad-062148925e2f.png)

### Load
One step before the loading - was to create the schema for our loading tables in pgAdmin

![alt text](level-1/images/pet_products_db_schema.png)

After the schema was created - we were able to move to the loading process

![image](https://user-images.githubusercontent.com/98370960/191398614-91ec0791-6dc4-41c5-a299-813d17644180.png)

Checking that load was successful in pgAdmin (one example)

![alt text](level-1/images/pet_prod_review_id_table_query.png)

## ETL Process: Digital Video Games Dataset
### Extract
* Extracted dataset:  https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Digital_Video_Games_v1_00.tsv.gz
* Extracted number or records: 145,431
![image](https://user-images.githubusercontent.com/98370960/191395136-ce8f44ff-1eda-4e67-a344-40057995c565.png)

### Transform
![image](https://user-images.githubusercontent.com/98370960/191395256-211e3d5b-82e8-4cdd-9b6a-06b40c23bae1.png)
![image](https://user-images.githubusercontent.com/98370960/191395324-a4fb8469-96a4-4900-8f10-a15f954fad2f.png)
![image](https://user-images.githubusercontent.com/98370960/191395387-f39d6cb5-3ed9-42eb-be44-0ca111f39263.png)
![image](https://user-images.githubusercontent.com/98370960/191395576-e0c92f71-7644-46a8-85de-bb2f5f447454.png)
![image](https://user-images.githubusercontent.com/98370960/191395654-f320d517-5671-4562-8731-8fa1543ff6c1.png)

### Load
One step before the loading - was to create the schema for our loading tables in pgAdmin

![alt text](level-1/images/dvg_schema.png)

After the schema was created - we were able to move to the loading process

![image](https://user-images.githubusercontent.com/98370960/191398407-91e8ef00-af57-4030-833e-2951fa2ffdfd.png)

Checking that load was successful in pgAdmin (one example)

![alt text](level-1/images/dvg_review_id_query.png)









