# Wrangling and Analysis of WeRateDogs

## Dataset

WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog. These ratings almost always have a denominator of 10 with the numerators almost always greater than 10 (because they're good dogs).  

The datasets used were gathered from a compiled archive containing basic tweet data for over 5000 of WeRateDogs tweets, querying Twitter's API to gather more tweet data from the WeRateDogs account, and an image prediction file containing prediction data gotten from running images of dogs from the archive through a neural network that can classify breeds of dog.

The datasets were then read in dataframes and assesed visually and programmatically after which the tidiness and data quality isssues were addressed. Some of the issues addressed include false breed predictions by the neural network, dog stages represented in more than a column, incorrect dog names, disorganized prediction algorithm confidence, unessential features, nulls as well as duplicates. After wrangling, the resulting dataset had 13 features of about 1700 tweets.

## Summary of Findings

Although more focus was placed on wrangling, some of the insights gotten fom exploration are given below:
* There was actually a strong positive correlation between the amount of likes a rating tweet got and the amount of retweets on it.
* Each dog rating tweet by the WeRateDogs account had 9288 likes and 2834 retweets on an average.
* Amongst the 4 dog stages tweeted, dogs in the pupper stage got tweeted and rated regularly. They were followed by dogs in doggo, puppo and floofer stages respectively.
* A lakeland terrier with a rating of 13/10 was the most liked dog with approximately 133k likes.
* The highest rating was 165 which was unusual given the mean rating was 13. On further inspection, it was discovered that the rating was given to a group of dogs in one image.
* The breed predictions were made with an average algorithm confidence of 55.2%.
