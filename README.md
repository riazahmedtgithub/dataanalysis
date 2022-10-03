# **DataAnalysis project:**

**Synopsis:**
        Used a daset from Kaggle to prove my data manipulation skill in python panda dataframes and matplotlib/sns libraries.  The result can be obtained by various means and I have tried to include a variety of methods for diversification.

**Input Used:**
        netflix-popular-movies-dataset/n_movies.csv dataset from kaggle
        
**Tools Used:**
        Python pandas, matplotlib, sns

**Brief overview:**

Data cleansing:

1. Imported the required libraries
2. Read the file and load in a dataframe
3. Inspect the dataframe indexes and columns
4. Dropped the year column with NaN values.
5. For the missing values in certificate column, I have used the backfill method to fill up.
6. The year column contains data like "2014-1015". I have just used the first mentioned year in the year column and striped all the following characters by using str method.  Also, only the numerical rows are selected using regex functionality.
7. Total number of films released in a year has been found out using the value_counts()method and a matplotlib plot has been plotted.
8. Sorting the dataset by duration of the movie in descending order,  top 10 longest movies has been found.
9. Using the condition expression, we have got the rows only for the certificate TV-MA out of the result from point 8.
10. Using the loc method, movies with the rating of 4.4 and year released in 2019 and 2021 has been found for certificate "TV-MA".
11. Lambda function has been used to find the genre only in 'Comedy','Drama' out of the various categories.
12. Apply method has been used to introduce a recommendation column to watch movies if the rating is more than 5.  

Plotting:

1.  Plotted the total number of films released by the year.
2.  Histogram of ratings has been plotted.
3.  Count plot of recommendation vs skip movies.

**Analysis:**

        As seen from the histogram graph, we can find  most of the movies had rating between 6 and 8.
        From the count polot, the recommendable movies are comparably higher than the skipped ones.
        As seen from the graph, we can find the number of movies increased significantly only from 2013
