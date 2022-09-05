# WeRateDogs Twitter Archive Data Wrangling Project

## by Christabel Onwuka


## Introduction

This is my second project in the Udacity/ALX-T Data Analyst Nanodegree Program which was focused on the data wrangling process. In this project, Wrangle and Analyze Data, I used Python and its libraries, to gather data from a variety of sources and in a variety of formats, assessed its quality and tidiness, and then cleaned it in a process called data wrangling. I documented my wrangling efforts in a Jupyter Notebook, and showcased them through analyses and visualizations using Python (and its libraries).

## Dataset
 
The dataset wrangled, analyzed and visualized is the tweet archive of Twitter user [@dog_rates](https://twitter.com/dog_rates), also known as [WeRateDogs](https://en.wikipedia.org/wiki/WeRateDogs), a Twitter account that rates people's dogs with a humorous comment about the dog. A popular Twitter account with more than 9 million followers, [@dog_rates](https://twitter.com/dog_rates) has been featured extensively in the international media.

For this project, I worked with these three pieces of data:

-  WeRateDogs' Twitter archive data (`twitter_archive_enhanced.csv`) which they downloaded and sent it to Udacity via email exclusively for use in this project. This archive contains basic tweet data (tweet ID, timestamp, text, etc.) for all 5000+ of their tweets as they stood on August 1, 2017. I downloaded this data manually from the Udacity workspace.

- The second piece of data, the tweet image prediction file (`image_predictions.tsv`) was programmatically downloaded using the url provided on the Udacity workspace.

- For the third piece of data, I used the `tweet_json.txt` file provided in the workspace by Udacity pending the authentication of Twitter API access. 



## Summary of Findings

After wrangling and exploration the data, some of the insights uncovered include:

1. Of the 306 dogs with defined dog stages, ***the dog stage, `pupper`, is the most popular*** with more than 200 dogs (about 70%) listed as pupper, followed by doggo at about 21% and puppo at ~ 8%.

2. ***On average people were likely to rate their dogs 12 out 10 as in 12/10***.

3. ***The p1 image prediction algorithm was most likely to be True for most dog images*** with original tweets in the third quartile(75%) having an algorithm prediction confidence level of about 85%. 

4. Of the 1994 dogs with image predictions, about ***32% are without names***. The remaining 68% have names.

 
## Resources used:

 - For updated exception error to gather data from API: *[Tweepy](https://docs.tweepy.org/en/stable/exceptions.html)* and *[TweepError](https://stackoverflow.com/questions/68412800/tweeperror-attribute-error-when-using-tweepy)*.

 - Template for code used to read tweet_json.txt to a dataframe gotten from [Ademola Oladapo](https://alx-nd-c1.slack.com/archives/C03CRB0V6J2/p1657271483905439?thread_ts=1657271081.343879&cid=C03CRB0V6J2) -- Data Analyst - Session Lead on Slack.

 - For extracting string(s) from a list used in extracting lower-case strings from the name column during wrangling, see [here](https://stackoverflow.com/questions/53935954/how-to-get-only-lowercase-strings-from-a-list-using-list-comprehension).
