# DSI-Project-3-Web-APIs-Classification

### Contents:
- [Problem Statement](#Problem-Statement)
- [Executive Summary](#Executive-Summary)
- [Conclusions and Recommendations](#Conclusions-and-Recommendations)

### Problem Statement 

Reddit is basically a large group of social news in which registered users can talk about almost anything you can imagine under "sub-reddit", a common place for people to share and discuss about any particular topic, from news, to pop culture, to technology, to comics, to any relationship advices, or to the weirdest things in the world. Since there are more than 138,000 active subreddits, users are able to interact with contents called "posts" (which are titled, contain a main body of either text or media attachments, etc.) through comments and participate in all of them freely except private subreddits, which will be requried an admission process.

As there are extremely large posts on reddit, it is near to impossible to sort all the posts manually. Let's imagine What if a bug in the system or simple human error ends up corrupting sub-reddit tags? Then the tedious responsibility of fixing it befalls someone to read, understand, and classify the posts. This makes it difficult to simply glance and guess which sub-Reddit a given post belongs to.

This leads me to the problem: **"How accurately can we use machine learning to classify similar content from two different sources?"**

The aim of this project is to classify from 2 different subreddits, /r/Bitcoin and /r/dogecoin. I will scrape 1000 posts for each of the two sub-Reddits using Reddit’s API, clean our raw data by getting rid of irrelevant content, turn messy stuff of post-level data into a processable form, then train and test out 3 different classification models (Random Forest, Naive Bayes Classifier, Logistic Regression) which will be evaluated based on accuracy scores, as we are only concerned about whether or not a post is correctly classified since Bitcoin and dogecoin are so many in common, investors or anyone interested in both can misunderstand and lead to investment mistakes in the future. This will help them to post in the correct subreddit and be able to get more useful help from comments.


### Executive Summary




### Conclusions and Recommendations


