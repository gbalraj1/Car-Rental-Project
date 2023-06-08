# Car-Rental-Project for Data Engineering Capstone Project 
# Wandererz car rental system
## This project is a complete data Pipeline project for a car rental service using AWS resources. 
1. It starts with the generation of test raw data in csv files for the locations, staff members, customers, car inventory, car models, reservations and rentals using Python code and other methods
2. The raw data from the local system is EXTRACTed into an RDS Database
3. The CSV files are moved from RDS to S3 using a glue job
4. A Glue Crawler is used to create a Glue data catalog for the CSV Files
5. A Glue Job was used to Transform the CSV files to Parquet files and put into S3 for increased processing speed
6. A Glue Crawler was used to create a data catalog for the Parquet Files
7. A Glue Job was used to TRANSFORM files and createan analysis parquet file ,joining the fields needed to analyse which type of cars are in demand at each location, and added to Glue Catalog
9. Athena was used to query and check if the tables values were transferred accurately
10. Created a DATA LAKE and added users with different level of permissions to access it
11. A Redshift cluster was created data LOADED from data lake to the data warehouse using external tables needed for the data analysis
12. The bar graphs were generated using MATPLOT LIB and pandas data frames in the JUPYTER Notebook.
