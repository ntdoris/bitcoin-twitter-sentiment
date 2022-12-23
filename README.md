# Flatiron Phase 4 Project: Classifying Bitcoin Tweet Sentiment

## Project Overview & Objective

This project seeks to build a model that accurately classifies tweets about Bitcoin as having either positive or negative sentiment. Unlabeled tweets classified by this model could ultimately could be used to analyze time trends on Bitcoin sentiment and assess the predictive power of Twitter sentiment on future price movements of the cryptocurrency.

## The Data

This project uses Twitter data sourced from [Kaggle](https://www.kaggle.com/datasets/gautamchettiar/bitcoin-sentiment-analysis-twitter-data?resource=download). It consists of 1 million Tweets referencing Bitcoin between February and August 2021. The sentiment is pre-labeled.

## Modeling

### Target

* In this analysis we target sentiment - positive or negative.
* Sentiment is fairly balanced, with around 53 percent of tweets labeled as negative and 47 percent positive.
![image](https://github.com/ntdoris/dsc-project-4/blob/main/images/tweet_distribution.png)

### Evaluation Metrics

* As the data is fairly balanced and we value false positives and false negatives equally, we focus on F1 score and accuracy

### Final Model: 

* Achieved 97 percent F1 score, 97 percent accuracy
![image](https://github.com/ntdoris/dsc-project-4/blob/main/images/model_f1_comp.png)
![image](https://github.com/ntdoris/dsc-project-4/blob/main/images/model_ac_comp.png)

* Most important features in positive tweets include:
![image](https://github.com/ntdoris/dsc-project-4/blob/main/images/feat_importance_pos20.png)

* Most important features in negative tweets include:
![image](https://github.com/ntdoris/dsc-project-4/blob/main/images/feat_importance_neg20.png)

* Just 3 percent of validation data categorized as negative when it was actually positive
* Just 1.8 percent of validation data categorized as positive when it was actually negative

![image](https://github.com/ntdoris/dsc-project-4/blob/main/images/final_confusion_matrix_normalized.png)

## Conclusion

* A Logistic Regression model was the best-performing classifier, with Count Vectorization used to process the annotated tweets
* Final model can classify unlabeled Tweets as positive or negative with ~97 percent accuracy, 97 percent F1 score
* Words important to the model included ?best?, ?awesome?, ?successful?, ?insane?, ?worst?, ?worthless?
* Positive tweets had more hashtags on average, negative tweets more frequently contained a price


### Next Steps / Recommendations

* Pull more recent Tweets on Bitcoin via Twitter API and run final model on real-time data
* Use model-labeled Tweets to conduct Time Series Analysis, with the aim of understanding the predictive power of Tweet sentiment on the price of BTC
![image](https://github.com/ntdoris/dsc-project-4/blob/main/images/tweet_sentiment_vs_bitcoin_px.png)
![image](https://github.com/ntdoris/dsc-project-4/blob/main/images/tweet_volume_vs_bitcoin_px.png)

## For More Information

* [Notebook](https://github.com/ntdoris/dsc-project-4/blob/main/project4.ipynb)
* [Presentation](https://github.com/ntdoris/dsc-project-4/blob/main/presentation.pdf)
* Reach me at ntdoris2@gmail.com

