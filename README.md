# SQL-data-cleaning
This is an educational project on data cleaning and preparation using SQL. The original database in CSV format is located in the file club_member_info.csv. Here, we will explore the steps that need to be applied to obtain a cleansed version of the dataset.
### Inspect the initial data:


 
## This is the code to explore data
'''sql
SELECT * FROM table LIMIT 10;
'''
Result:






### Cleaning Step 1
Detect null value
'''sql
SELECT COUNT(*) FROM club_member_info_cleanned WHERE marital_status IS NULL;
'''
Indentify MODE value in marital_status
'''sql
SELECT MODE(marital_status) FROM club_member
Replace null with MODE value
