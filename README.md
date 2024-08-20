# Home_Sales

This project leverages PySpark and Spark SQL on Google Colab to analyze home sales data and extract key metrics. The analysis involves creating temporary views, partitioning data, and managing temporary tables through caching and uncaching.

For instance, a table was generated with two columns: one displaying the average price (rounded to two decimal places) of four-bedroom homes, and the other grouping the years in which these properties were sold. Additionally, the project compares query runtimes across three scenarios: using an uncached temporary table, a cached temporary table, and a cached and partitioned temporary table stored in Parquet format.

## Key Metrics:
Some of the key metrics determined in the analysis include:

- The average sale price of four-bedroom houses for each year.
- The average price of three-bedroom, three-bathroom homes for each year they were built.
- The average price of homes with three bedrooms, three bathrooms, two floors, and at least 2,000 square feet for each year.
- The "view" rating for homes priced at $350,000 or more.
