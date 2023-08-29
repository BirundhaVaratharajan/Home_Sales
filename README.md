# Home_Sales

In this challenge, SparkSQL is used to determine key metrics about home sales data. Then using Spark to create temporary views, partition the data, cache and uncache a temporary table.
Finally verified that the table has been uncached.

Using SparkSQL following questions have been answered

1.What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.


|year|4Bed_Average_price|

|2019|          300263.7|

|2020|         298353.78|

|2021|         301819.44|

|2022|         296363.88



2.What is the average price of a home for each year it was built that has three bedrooms and three bathrooms? Round off your answer to two decimal places.

date_built|3Bed_Average_price|
+----------+------------------+
|      2010|         292859.62|
|      2011|         291117.47|
|      2012|         293683.19|
|      2013|         295962.27|
|      2014|         290852.27|
|      2015|          288770.3|
|      2016|         290555.07|
|      2017|         292676.79


3.What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.

date_built|2floor_Average_price|
+----------+--------------------+
|      2010|           285010.22|
|      2011|           276553.81|
|      2012|           307539.97|
|      2013|           303676.79|
|      2014|           298264.72|
|      2015|           297609.97|
|      2016|            293965.1|
|      2017|           280317.58|



4.What is the "view" rating for homes costing more than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.


view|Average_price|
+----+-------------+
|  51|    788128.21|
|  54|    798684.82|
|  69|    750537.94|
|  87|    1072285.2|
|  73|    752861.18|
|  64|    767036.67|
|  59|     791453.0|
|  85|   1056336.74|
|  52|    733780.26|
|  71|     775651.1|
|  98|   1053739.33|
|  99|   1061201.42|
|  96|   1017815.92|
| 100|    1026669.5|
|  70|    695865.58|
|  61|    746877.59|
|  75|   1114042.94|
|  78|   1080649.37|
|  89|   1107839.15|
|  77|   1076205.56|
+----+-------------+
only showing top 20 rows
