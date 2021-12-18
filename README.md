# Information-Retrival

This project aimed to predict the sentiments of tweets scraped from business news twitter accounts. Through this project, we want to create a retrival system and ranking systems that determines whether or not a piece of information is objective through Subjectivity detection and the tone through Polarity Detection. 

## Subjectivity Detection 
For subjectivity, we want to know if a tweet is objective or neutral. 

## Polarity Detection
Polarity is assigned to a tweet that is objective and we futher determine if the tone is positive or negative.

## Classification Methods 
We achieve classification by testing a variety of machine learning models and deep learning models. The models that we have used in our classification includes Multinomial Naive Bayes, Random Forest Classifier, Gradient Boosting Classifier, Multi-layer Perceptron (MLP) Classifier, Support Vector Machine (SVM) Classifier and Logistic Regression.

Overall, we observed that all methods in general had an accuracy of ~70%. But MLP and SVM gave some of the best results among all the methods listed. It is also note worthy to consider the scalability and longevity of using a unsupervised model like SVM vs MLP. Given that MLP had the same performce as SVM, this means that it is possible to cut out the labelling step in pre-processing and thus making workflow more efficient. 


# Labelling of Tweets 
Two members in the team were tasked with labelled the records and below is an overview of the labelled data: 

    Number of labelled tweets: 2164 / 14060 (~15% labelled)

    Number of opinionated tweets: 1015 (~47 % opinionated, ~53% neutral)

    Positive to Negative ratio: 550:465 (~54:46)

Every Tweet was labelled to be either "Opinionated" (O) or "Neutral" (NT). If the tweet is "Opinionated", it would have a "Positive" (P) tone or a "Negative" (N) tone. 

    If a tweet is "Opinionated" and "Negative", it is labelled ON

    If a tweet is "Opinionated" and "Positive", it is labelled OP

    If a tweet is "Neutral", it labelled NT
