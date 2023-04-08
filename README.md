# Home_Sales

In this challenge, you'll use your knowledge of SparkSQL to determine key metrics about home sales data. Then you'll use Spark to create temporary views, partition the data, cache and uncache a temporary table, and verify that the table has been uncached.

* Import the necessary PySpark SQL functions for this assignment.

* Read the home_sales_revised.csv data in the starter code into a Spark DataFrame.
https://2u-data-curriculum-team.s3.amazonaws.com/dataviz-classroom/v1.2/22-big-data/home_sales_revised.csv

* Create a temporary table called home_sales.

* Answer the following questions using SparkSQL:

* What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.
* 
![image](https://user-images.githubusercontent.com/12514249/230746448-95a35e08-9214-46cc-afc3-e8e5bd5b746f.png)

* What is the average price of a home for each year it was built that has three bedrooms and three bathrooms? Round off your answer to two decimal places.
* 
 ![image](https://user-images.githubusercontent.com/12514249/230746472-96078cf0-9a15-405c-8ca0-6cbff238ce4d.png)

* What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.
* 
 ![image](https://user-images.githubusercontent.com/12514249/230746487-626540d5-d2a7-4837-8fff-2d63dce45108.png)

* What is the "view" rating for homes costing more than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.
* 
![image](https://user-images.githubusercontent.com/12514249/230746497-5e817b0f-51e0-4ad7-aa0d-b4fd2b2811a4.png)

* Cache your temporary table home_sales.

* Check if your temporary table is cached.

* Using the cached data, run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.
* 
 ![image](https://user-images.githubusercontent.com/12514249/230746524-3cb2ec95-407c-4ca2-b94e-2f85192cee91.png)

* Partition by the "date_built" field on the formatted parquet home sales data.

* Create a temporary table for the parquet data.

* Run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.
* 
 ![image](https://user-images.githubusercontent.com/12514249/230746558-2cf1068b-99bc-453c-ba75-7c107b2119f6.png)

* Uncache the home_sales temporary table.

* Verify that the home_sales temporary table is uncached using PySpark.

* Download your Home_Sales.ipynb file and upload it into your "Home_Sales" GitHub repository.


# Requirements
A Spark DataFrame is created from the dataset. 

A temporary table of the original DataFrame is created. 

A query is written that returns the average price, rounded to two decimal places, for a four-bedroom house that was sold in each year. 

A query is written that returns the average price, rounded to two decimal places, of a home that has three bedrooms and three bathrooms. 

A query is written that returns the average price of a home with three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet for each year built rounded to two decimal places. 

A query is written that returns the view rating for the average price for homes that are greater than or equal to $350,000, rounded to two decimal places. (The output shows the run time for this query.) 

A cache of the temporary "home_sales" table is created and validated. 

The query from step 6 is run on the cached temporary table, and the run time is computed. 

A partition of the home sales dataset by the "date_built" field is created, and the formatted parquet data is read. 

A temporary table of the parquet data is created. 

The query from step 6 is run on the parquet temporary table, and the run time is computed. 

The "home_sales" temporary table is uncached and verified. 

