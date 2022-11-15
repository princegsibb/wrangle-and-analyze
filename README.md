# wrangle-and-analyze

This project was developed as a part of the course on Data Wrangling, during Udacity's Data Analytics Nanodegree program. This project makes use of the Twitter Archive of WeRateDogs and additional information about the tweets, to perform Data Wrangling & Data Analysis and Visualisation.

Datasets Used

1️. WeRateDogs Twitter Archive : This file contains the tweet archive of @WeRateDogs. This file is treated as on-hand file, and is available in this repository.
2️. Image Prediction Dataset : This file is a TSV file, which contains the Top 3 predictions of a Dog's Breed, and is downloaded using Python's Requests library from the cloud.
3️. Tweets Additional Info Dataset : This dataset is created using the Tweepy API, which allows to get access to the information about the particular in JSON format. This JSON output is formatted and compiled into a CSV file.

Data Quality Tasks Identified

The datatype of Timestamp is incorrect, should be datetime datatype.
Remove All Tweets from Tweet Archive Dataframe, which have incorrect Tweets IDs.
Replace Missing Name values in name represented by None with NaN.
Replace the illogical values a, by, the, an, all, just, very in the name column with NaN, to represent Invalid values.
Replace Missing Values in doggo, floofer, pupper and puppo with NaN.
Remove All Tweets which are Retweets.
Remove All Tweets which are Reply Tweets.
Remove All Tweets from Tweet Archive which do not have an image.
Remove Tweets which have Numerators = 420, 1776, 960, 666, and Denominator = 7, as they are not rating tweets, and thus invalid.
Incorrect Numerator and Denominator values in tweet with (1,2). Replace them by correct rating of (9,10).
Extraction of Short URLs from Tweet text column, and placing into new column called short_url.
Data Tidiness Tasks Identified
Melt the columns doggo, floofer, pupper and puppo into a single column.
Multiple Columns in Image Prediciton dataframe, to represent the dog breed, change to representation in a single column.
Merge the Tweet Archive, Image Prediction and Additional Information for every unique tweet into a single dataframe.
