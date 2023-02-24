# Twitter-Scraping
Twitter Scraping_capstone
**By using the “snscrape” Library, Scrape the twitter data from "https://medium.com/dataseries/how-to-scrape-millions-of-tweets-using-snscrape-195ee3594721" using Python
**

Create a dataframe with date, id, url, tweet content, user,reply count, retweet count,language, source
Here, we've added a few new columns to the list that we're appending to tweets_list: tweet.url, tweet.replyCount, tweet.retweetCount, tweet.lang, and tweet.sourceLabel. We've also converted the tweet.date object to a string with a specific format using the strftime method.
Finally, we've updated the column names in the DataFrame constructor to match the new column names.

**Store each collection of data into a document into Mongodb along with the hashtag or key word we use to  Scrape from twitter. 
**

Here, we've added a new parameter keyword to the function, and included it in the list of columns that we're appending to tweets_list. We've also added a new column to the DataFrame called "Keyword". This will scrape the tweets from the given URL, add the keyword to each tweet as a new column, and insert the tweets into MongoDB using the insert_many method of the collection.

**Create a GUI using streamlit that should contain the feature to enter the keyword or Hashtag to be searched, select the date range and limit the tweet count need to be scraped. After scraping, the data needs to be displayed in the page and need a button to upload the data into Database and download the data into csv and json format.
**

This function takes in the keyword, start date, end date, and tweet count as inputs, and scrapes tweets using the sntwitter library. It then creates a pandas DataFrame with the scraped tweets and inserts them into MongoDB using the insert_many method.
