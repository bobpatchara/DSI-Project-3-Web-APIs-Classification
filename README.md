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

### Models Train/Test Score Comparison Table
| Models | CVEC(Train score) | CVEC(Test score) | Diff(%) | Tfidf (Train score) | Tfidf(Test score) | Diff(%) |
| --- | --- | --- | --- | --- |--- | --- |
| Baseline | 54.68% | 54.68% | - | 54.68% | 54.68% | - |
| Random Forest |75.45% | 74.27% | 1.18% | 75.37% | 74.51% | 0.86% |
| Logistic Regreesion | 79.50% | **79.85%** | **0.35%** | 80.63% | 79.37% | 1.26% |
| Naive Bayes | 81.20% | **80.34%** | **0.86%** | 80.71% | 79.61% | 1.1% |
| Supporting Vector Machine | 74.80% | 73.79% | 1.01% | 77.23%| 77.43% | 0.20% |


### Classification Matrix Table
| Evaluation Metrics | Model 1: Random Forest | Model 2: Logistic Regression | Model 3: Navie Bayes |Model 4: Supporting Vector Machine |
| --- | --- | --- | --- | --- |
| Accuracy | 74.51% | **79.85%** | **80.34%** | 77.43% | 
| Sensitivity | 54.55% | 66.84% | 78.61% | 81.82% | 
| Specificity | 91.11% | 90.67% | 81.78% | 73.78% | 
| Precision | 83.61% | 85.62% | 78.19% | 72.17% | 

All four models (Random Forest, Logistic Regression, Naive Bayes, and Support Vector Machine) exceed the baseline accuracy of 54.68% by at least 1.3x as almost models performed with an accuracy greater than 75% except Random Forest, demonstrating strong ability to classify at least 3 in 4 posts into the correct subreddit. However, the winner was definitely **the Multinomial Naive Bayes model, which was able to correctly 4 in 5 posts or 80.34%**. This is within expectation because the topics of two chosen subreddits are quite similar. 

Therefore, this is the model we would recommend Reddit Data Team to implement to help them classify error/buggy posts that have lost their subreddit tags and also help users, investors or anyone who interested in both subreddits preventing misunderstand and to not make investment mistakes in crptocurrency trading in the future.

Further improvements for the model include:

- Collecting more training data not only just Text data but also Pic posted in a post as a feature to classify subreddits.
- Enhancing the model's ability to classify more than two subreddits in our classification model. 
- Tuning of parameters for any models to get a better score. However, this requires a longer amount of time to tune to get the perfect parameters.


