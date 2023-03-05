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

The project folder also includes:
- dataset files as explained in *Context* section
- .csv files with feature importance for each of the models
- .xlsx file with information on f1 scores of the models


 ## References
  
- [Feature Importance and Feature Selection With XGBoost in Python](https://machinelearningmastery.com/feature-importance-and-feature-selection-with-xgboost-in-python)

- [Feature importance for VotingClassifers?](https://github.com/scikit-learn/scikit-learn/discussions/22569)

- [How to set center color in heatmap](https://stackoverflow.com/questions/56536419/how-to-set-center-color-in-heatmap)

- [11 Ways to Get Visitors to Spend More Time on Your Website](https://www.entrepreneur.com/science-technology/11-ways-to-get-visitors-to-spend-more-time-on-your-website/418094)
