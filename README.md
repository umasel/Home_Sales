# Home_Sales

This project leverages PySpark and Spark SQL on Google Colab to analyze home sales data and extract key metrics. The analysis involves creating temporary views, partitioning data, and managing temporary tables through caching and uncaching.

For instance, a table was generated with two columns: one displaying the average price (rounded to two decimal places) of four-bedroom homes, and the other grouping the years in which these properties were sold. Additionally, the project compares query runtimes across three scenarios: using an uncached temporary table, a cached temporary table, and a cached and partitioned temporary table stored in Parquet format.

## Key Metrics:
Some of the key metrics determined in the analysis include:

- The average sale price of four-bedroom houses for each year.
- The average price of three-bedroom, three-bathroom homes for each year they were built.
- The average price of homes with three bedrooms, three bathrooms, two floors, and at least 2,000 square feet for each year.
- The "view" rating for homes priced at $350,000 or more.

## Requirements
A Spark DataFrame is created from the dataset. (5 points)

A temporary table of the original DataFrame is created. (10 points)

A query is written that returns the average price, rounded to two decimal places, for a four-bedroom house that was sold in each year. (5 points)

A query is written that returns the average price, rounded to two decimal places, of a home that has three bedrooms and three bathrooms. (5 points)

A query is written that returns the average price of a home with three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet for each year built rounded to two decimal places. (5 points)

A query is written that returns the view rating for the average price for homes that are greater than or equal to $350,000, rounded to two decimal places. (The output shows the run time for this query.) (10 points)

A cache of the temporary "home_sales" table is created and validated. (10 points)

The query from step 6 is run on the cached temporary table, and the run time is computed. (10 points)

A partition of the home sales dataset by the "date_built" field is created, and the formatted parquet data is read. (10 points)

A temporary table of the parquet data is created. (10 points)

The query from step 6 is run on the parquet temporary table, and the run time is computed. (10 points)

The "home_sales" temporary table is uncached and verified. (10 points)
