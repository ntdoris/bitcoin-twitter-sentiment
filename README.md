# Flatiron Phase 4 Project

## Project Overview & Business Problem

In this project, we help Crypto Consultancy firm X build a model that can accurately classify Tweets about Bitcoin as having either positive or negative sentiment. Firm X would like to use the model to classify unlabeled Tweets and understand any characteristics distinguishing the positive and negative Tweets. 

## The Data

This project uses Twitter data sourced from Kaggle. It consists of 1 million Tweets referencing Bitcoin between February and August 2021. The sentiment is pre-labeled.

## Modeling

### Target

* In this analysis we target sentiment - positive or negative.
* Sentiment is fairly balanced, with around 52 percent of tweets labeled as positive and 48% negative.

### Evaluation Metrics

* As the data is fairly balanced, we focus on F1 score and accuracy

### Final Model: 

* Achieved 80 percent recall, 73 percent ROC AUC score, 72 percent accuracy

![Screen Shot 2022-12-15 at 2 33 11 PM](https://user-images.githubusercontent.com/102126161/207950596-6972a96b-7ca2-4ef4-80bc-a3e1c550a653.png)


## Conclusion


* Period of higher Twitter volume associated with period of lower Bitcoin price


* Spike in positive sentiment occurred around same time as rise in Bitcoin price


* Positive sentiment Tweets tend to have more hashtags on average


* Final model can classify unlabeled Tweets as positive or negative with ~90% accuracy


### Next Steps

* Pull more recent Tweets on Bitcoin via Twitter API
* Run final model on unseen data, i.e. new Tweets
* Use model-labeled Tweets to conduct Time Series Analysis, with the aim of understanding the predictive power of Tweet sentiment on the price of BTC
* Use deep learning models to classify Tweets, comparing these results to previous model

## For More Information

* [Notebook](https://github.com/ntdoris/dsc-project-4/blob/main/project4.ipynb)
* [Presentation](https://github.com/ntdoris/dsc-project-4/blob/main/presentation.pdf)
* For more information, you can reach me at ntdoris2@gmail.com

