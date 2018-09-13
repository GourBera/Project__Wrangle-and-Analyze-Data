Gathering data- Access tweet data of @dog_rates using tweeter API | Assessing data- finding various Quality and Tidiness issues in data | Cleaning data- Defining cleaning steps and finally cleaning all issues present in our data | Visualizing and Reporting- Visualizing various insight and finally creating detail report.


# Wrangling, Analyzing and Visualizing Data

Data wrangling, which consists of:
  1. Gathering data
  2. Aessing data
  3. Cleaning data
  
Storing, analyzing, and visualizing our wrangled data
Reporting on 1) our data wrangling efforts and 2) our data analyses and visualizations

# Quality issues

  1. Could not fetch data from Twitter API for some tweet_ids
  2. Type of 'timestamp' column in df_clean is Object instead of timestamp
  3. Possible incorrect data in 'name' column like- 'a', 'the', 'this'
  4. 'numerator' and 'denominator' columns have some unusual values
  5. column name 'id' in tweet_df_clean DataFrame should be changed to 'tweet_id' in-order to merge with other DataFrame
  6. Missing values in images_clean DataFrame (2075 rows instead of 2356)
  7. We have null values in various column
  8. Type of Various column like in_reply_to_status_id, in_reply_to_user_id, retweeted_status_id, retweeted_status_user_id in tweet_df_clean DataFrame is Float instead of Int
  9. Some tweet_ids does not actually contain a picture of dog like- (666052000000000000,666412000000000000)
  10. Calculate rating based on 'numerator' and 'denominator'

# Tidiness issues
  1. Various unwanted columns in df_clean, and tweet_df_clean DataFrame
  2. We can have one column 'dog_stage' instead of doggo floofer pupper and puppo
  3. df_clean, images_clean and tweet_df_clean should be merged to one DataFrame


# Define Steps and Cleaning data
  1. Convert column 'timestamp' from Object to timestamp
  2. Rename all possible incorrect name to NaN
  3. Rename column 'id' to 'tweet_id'
  4. Drop all unwanted column from all 3 DataFrame
  5. Create one column 'dog_stage' instead of doggo floofer pupper and puppo
  6. Create column 'rating' to calculate rating based on 'numerator' and 'denominator'
  7. Merge all 3 DataFrame








