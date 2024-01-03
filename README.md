# nosql-challenge

## Part1_Starter_SetUp - UK Food Hygiene Ratings Analysis

The Jupyter notebook imports MongoDB and connects to a database containing UK food hygiene ratings data. It explores the `establishments` collection in the `uk_food` database.

The notebook conducts initial exploration of the data, printing out a sample document. The database is then updated in several ways:

- Inserts a new restaurant document for an unrated restaurant called "Penang Flavours"
- Looks up and adds the correct BusinessTypeID for the restaurant category
- Removes all establishments located in the Dover Local Authority area
- Converts latitude, longitude, and RatingValue fields from strings to numeric data types for easier analysis

In the end, you have a cleaned database ready for further analysis and visualizations into UK food hygiene ratings.

The notebook provides a template for connecting to MongoDB, exploring a new dataset, and cleaning documents in preparation for analysis.

## Part2_NoSQL_Analysis - UK Food Hygiene Analysis with MongoDB and Pandas

This code imports MongoDB and Pandas to connect to a database of UK food hygiene ratings, analyze the data, and output results.

It starts by connecting to a MongoDB database called `uk_food` and accessing the `establishments` collection.

Some initial queries filter the data and output sample documents, converting results to Pandas DataFrames for analysis. Queries search for:

- Establishments with a hygiene score of 20
- Establishments in London with a rating greater than or equal to 4 
- A specific restaurant called "Penang Flavours"

The code then searches for top rated establishments near Penang Flavours and sorts the results.

Finally, an aggregation pipeline is constructed that matches, groups, and sorts establishments with a hygiene score of 0 by Local Authority. This pipeline output is also converted to a Pandas DataFrame.

In the end, you have code to connect MongoDB and Pandas for food hygiene data analysis. The queries and aggregations provide examples of filtering, projecting, sorting, limiting, grouping, and aggregating data as part of an analysis workflow.