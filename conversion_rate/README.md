# <p align="center">Conversion Rate Challenge</p>

<p align="center"> <img src="dsw_logo.png.png" width="250"> </p>

## Context 

Data Science Weekly www.datascienceweekly.org is a f by independent data scientists. The data scientists who created the newsletter would like to understand better the behaviour of the users visiting their website. They would like to know if it's possible to build a model that predicts if a given user will subscribe to the newsletter, by using just a few information about the user. They would like to analyze the parameters of the model to highlight features that are important to explain the behaviour of the users, and maybe discover a new lever for action to improve the newsletter's conversion rate.

They designed a competition aiming at building a model that allows to predict the conversions (i.e. when a user will subscribe to the newsletter). To do so, they open-sourced a dataset containing some data about the traffic on their website. To assess the rankings of the different competing teams, they decided to use the f1-score.

The dataset (.csv file) is included in project folder. 

## Goals of the project
 - Explore the dataset and create come data visualisations
 - Train a baseline linear regression model
 - Train a regularized regression model


 ## Project files
The project includes several files:

1. Exploraroty data analysis 

        0_Conversion_rate_challenge_EDA.ipynb

2. Training several supervised machine learning models:

        1_Conversion_rate_challenge_LogReg_Multivariate.ipynb
        2_Conversion_rate_challenge_Adaboost_w_Decision_Trees.ipynb
        3_Conversion_rate_challenge_Xgboost.ipynb
        4_Conversion_rate_challenge_Voting_LogReg_Adaboost_tree_Xgboost.ipynb

3. Model performance comparison


    The notebook creates the file weather_forecast.csv in the working directory and saves it to S3 bucket.


3. Scraping information on hotels from booking.com


- Scraping Booking's search page to get hotel URLs and saving the resulting .json file to S3 bucket

        3a_booking_scraping_hotel_urls.py 
        3a_saving_hotel_urls_to_s3.ipynb


- Scraping hotel pages to get hotel name, coordinates, score given by users, text description and saving the resulting .json file to S3 bucket.

        3b_booking_scraping_hotels_data.py
        3b_saving_hotels_data_to_s3.ipynb



4. Creating a unique table with enriched information for hotels in each city and saving it so S3 bucket

        4_kayak_df.ipynb

5. Creating an SQL Database using AWS RDS

        5_creating_sql_database_in_rds.ipynb

6. Creating maps with top-5 cities in terms of weather and top-20 hotels in each of these cities

        6_maps.ipynb

 ## References

 - [Walmart Dataset on Kaggle](https://www.kaggle.com/datasets/yasserh/walmart-dataset) (dataset used in this project is based on the Kaggle dataset with modifications by Jedha).

- [How to check if any holiday is included in a time period in python](https://stackoverflow.com/questions/55388361/how-to-check-if-any-holiday-is-included-in-a-time-period-in-python)

- [Convert string month year (where year is only a two digits) to datetime in pandas](https://stackoverflow.com/questions/73288353/convert-string-month-year-where-year-is-only-a-two-digits-to-datetime-in-panda) 

- [Encoding features like month and hour as categorial or numeric?](https://datascience.stackexchange.com/questions/17759/encoding-features-like-month-and-hour-as-categorial-or-numeric)

- Photo by <a href="https://unsplash.com/@_gemmajade?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">gemma</a> on <a href="https://unsplash.com/photos/stpjHJGqZyw?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>
  