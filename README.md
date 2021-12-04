# Twitter_API_Data_Analysis

![](https://github.com/darraghmerrick/Twitter_API_Data_Analysis/blob/main/twitter.jpeg)
![](https://github.com/darraghmerrick/Twitter_API_Data_Analysis/blob/main/dog.jpeg)

This project performs wrangling and analysing of data, gathered from a variety of sources and in a variety of formats. The quality and tidiness was assessed, and then cleaned. Finally the wrangling results were show cased with insights and visualisations.
### Data Gathering

There are 3 sources of data for this project:

1. The 'twitter_archive_enhanced.csv' was directly download and put into the Jupyter notebook local directory.
WeRateDogs downloaded their Twitter archive and provided it to Udacity. This archive contains basic tweet data (tweet ID, timestamp, text, etc.) for all 5000+ of their tweets as they stood on August 1, 2017

2. The Image Predictions File 'image_prediction.tsv' is the output from when Udacity ran every image in the WeRateDogs Twitter archive through a neural network that can classify breeds of dogs. The results were a table full of image predictions (the top three only) alongside each tweet ID, image URL, and the image number that corresponded to the most confident prediction (numbered 1 to 4 since tweets can have up to four images).
This file had to be downloaded and written programmatically with python from the Jupyter notebook.

3. The additional data 'tweet_json.txt' was gathered from Twitter's API. We have the WeRateDogs Twitter archive and specifically the tweet IDs within it, so can gather this data for all 5000+ tweets. The twiter api download was one complete json dumped tweet with all the fields from tweepy downloaded data into tweet_json.txt. The relevant fields needed to be parsed and saved to a data frame, without duplicating columns we already have in other tables:

 All 3 data sets have the column "tweet_id" which will be used as the primary key to match the data to a row in the twitter-archive-enhanced.csv  and image_prediction.tsv.
 

The data needs to be analysed, cleaned and tidied.

When all 3 data sources are merged together, analyse it to get insights and create visualisations with Pandas and MatPlotLib

Report on the findings.
