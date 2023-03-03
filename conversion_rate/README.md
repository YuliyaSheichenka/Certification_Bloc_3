# <p align="center">Conversion Rate Challenge</p>

<p align="center"> <img src="dsw_logo.png" width="250"> </p>

## Context 

[Data Science Weekly](www.datascienceweekly.org) is a newsletters created by independent data scientists. These data scientists would like to understand better the behaviour of the users visiting their website. To do so, they open-sourced a dataset containing some data about the traffic on their website and held a competition aiming at building a machine learning model that allows to predict the conversions (i.e. when a user will subscribe to the newsletter). They would like to analyze the parameters of the model to highlight features that are important to explain the behaviour of the users, and maybe discover a new lever for action to improve the newsletter's conversion rate. To assess the rankings of the different competing teams, the site ownerss decided to use the f1-score.

The datasets used for this project include:
- labelled dataset (conversion_data_train.csv) that was separated into train that is used to train a model and the test to test the model. After the performance of a given model had been evaluated, the train and test parts of this labelled dataset were joined together again and the whole dataset was used for training the model once more.
- After such training, the model was used to make predictions on the unlabelled dataset (conversion_data_test.csv). The predictions of the model were sent to Jedha instructors who compared the predictions with the true labels and communicated the resulting f1-score. 

## Goals of the project

 - Do exploratory data analysis of the dataset
 - Train a baseline model
 - Improve the f1-score by training other models or by other means (feature engineering/selection, grid search, regularization...)
 - Analyse the parameters of the best model and give recommendations to improve the newsletter's conversion rate.


## Project files

The project includes several files:

1. Exploraroty data analysis

        0_Conversion_rate_challenge_EDA.ipynb

2. Training several supervised machine learning models 

        1_Conversion_rate_challenge_LogReg_Multivariate.ipynb (baseline model)
        2_Conversion_rate_challenge_Adaboost_w_Decision_Trees.ipynb
        3_Conversion_rate_challenge_Xgboost.ipynb
        4_Conversion_rate_challenge_Voting_LogReg_Adaboost_tree_Xgboost.ipynb

3. Model performance comparison

        5_Models_performance_comparison.ipynb

The file contains plots allowing to compare the f1-score of the models on the train part of the labelled dataset, on the test part of the labelled dataset, and on the test unlabelled dataset (this score was communicated by Jedha instructors who tested the model on the unlabelled dataset).


 ## References

 - [Walmart Dataset on Kaggle](https://www.kaggle.com/datasets/yasserh/walmart-dataset) (dataset used in this project is based on the Kaggle dataset with modifications by Jedha).

- [How to check if any holiday is included in a time period in python](https://stackoverflow.com/questions/55388361/how-to-check-if-any-holiday-is-included-in-a-time-period-in-python)

- [Convert string month year (where year is only a two digits) to datetime in pandas](https://stackoverflow.com/questions/73288353/convert-string-month-year-where-year-is-only-a-two-digits-to-datetime-in-panda) 

- [Encoding features like month and hour as categorial or numeric?](https://datascience.stackexchange.com/questions/17759/encoding-features-like-month-and-hour-as-categorial-or-numeric)

- Photo by <a href="https://unsplash.com/@_gemmajade?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">gemma</a> on <a href="https://unsplash.com/photos/stpjHJGqZyw?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>
  