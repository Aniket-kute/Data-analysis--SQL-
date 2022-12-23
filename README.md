# Basic Data-analysis--SQL-- cleaning project

### Using SQL to clean and analyze data and further visualize it using Power BI/ Tableau
Dataset: https://data.world/markbradbourne/rwfd-real-world-fake-data/workspace/file?filename=Call+Center.csv 

####Agenda : Import data into MYSQL Workbench -> Cleanse and Analyze in Workbench -> Visualize it in Power BI/ Tableau

 -----

**Step 1:**
_Importing the data:_ To check if the data is imported, I ran a select query to see the first 100 rows

**Step 2:**
_Cleaning the data:_ <br>
a. Date format: Change the date format to yyyy-MM-dd as this is the default format for MySQL. <br> 
&nbsp;&nbsp; How to fix: We use str_to_date function to convert the string to required date format. Before this we need to change the SQL_SAFE_UPDATES to 0 as we not using the where clause within the update command. next we turn back the safe update mode to 1 again <br> 
b. Empty values in customer_score column: Change empty values to NULL values. Use Update command and where clause to fill the empty values to null values.

**Step 3:** 
_Basic EDA:_ <br>
a. Finding the number of columns, rows of the table. <br>
b. Finding Distinct values in some of the columns. (Finding different channel of calls) <br>
c. Using Group By function to find the distribution of different categories of how the count of calls is distributed. <br>
d. Using Aggregate functions to find the min, max, average values for some of the columns (For call duration column) <br>
e. Using windows functions to analyze partitions within the data. (Used this to find the maximum call duration per day) <br>

**Step 4:**
_Tableau Visualization_



