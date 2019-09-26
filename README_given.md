# ![](https://Users/tricia/GA/projects/Reddit_NLP/images/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 3: Web APIs & Classification

### Problem Statement

More and more people are getting their news from social medias sites.   One-in-five U.S. adults say they often get news via social media. (https://www.pewresearch.org/fact-tank/2018/12/10/social-media-outpaces-print-newspapers-in-the-u-s-as-a-news-source/).  In a world of 'clicks' and associated dollars, it can be difficult to determine if a social media news story or any story for that matter, is real or made up.  

This project seeks to determine if you can accurately predict a fake or satire news story headline from a real news headline using Natural Language Programming and Reddit. 

### Summary

As of July 2019, Reddit is ranked as the No. 5 most visited website in U.S. and No. 13 in the world, according to Alexa Internet, with 55% of its user base coming from the United States, followed by the United Kingdom at 7.4% and Canada at 5.8%. (source:  https://en.wikipedia.org/wiki/Reddit)

Reddit is an American social news aggregation, web content rating, and discussion website. Posts are organized by subject into user-created boards called "subreddits", which cover a variety of topics including news, science, movies, video games, music, books, fitness, food, and image-sharing. (source:  https://en.wikipedia.org/wiki/Reddit) 

Data was collected utilzing two subreddits r/TheOnion - a satire site and r/nottheonion - a site that bills itself as real news stories that are so absurd they could be from TheOnion.  1000 headlines from both sites were used for a total of 2000 total headlines for training the model.  Using Countvecotorization to explore the data, a frequency list of TheOnion top words overlayed with the same words from nottheonion showed that the word 'new' was highly frequent in the satire site TheOnion while the word 'man' was more frequent for the real news site - nottheonion.  

![](/Users/tricia/GA/projects/Reddit_NLP/images/Onion_over_nottheonion.png)

Three models were explored. Logistic Regression, Multinomial Naive Bayes using Countvectorization and then the same using TF-IDF (Term Frequency - Inverse Document Frequency).  

It was determined after optimizing for sensitivity that a Multinomial Naive Bayes model using Countvectorization produced an accuracy score of 99.75% on brand new data.  

![](/Users/tricia/GA/projects/Reddit_NLP/images/final_confusion_matrix.png)


### Directory

1. Scraping and Cleaning
2. Exploratory Data Analysis
3. Modeling
    Model Logit Classifier
    Model Multinomial Naive Bayes using Countvectorization
    Model Multinomial Naive Bayes using TF-IDF 
4. Final Model using new data 





