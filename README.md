# Basic Data-analysis--SQL-- cleaning project

### Using SQL to clean and analyze data and further visualize it using Power BI/ Tableau
Dataset: https://data.world/markbradbourne/rwfd-real-world-fake-data/workspace/file?filename=Call+Center.csv 

####Agenda : Import data into MYSQL Workbench -> Cleanse and Analyze in Workbench -> Visualize it in Power BI/ Tableau

Step 1:
Importing the data: To check if the data is imported run a select query to see the first few rows

Step 2:
Cleaning the data: 
a. Date format: Change the date format to yyyy-MM-dd as this is the default format for MySQL.
    How to fix: We use str_to_date function to convert the string to required date format. Before this we need to change the SQL_SAFE_UPDATES to 0 as we not using the where clause within the update command. next we turn back the safe update mode to 1 again
b. Empty values in score column: Change empty values to NULL values. Use Update command and where clause to fill the empty values to null values.

Step 3: 
Basic EDA:
a. Finding the number of columns, rows of the table. 
b. Finding distinct values in some of the columns. 
c. Using group by function to find the distribution fo different categories of how the count of calls is distributed
d. 

