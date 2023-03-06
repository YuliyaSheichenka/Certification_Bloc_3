# <p align="center">Uber Pickups</p>

<p align="center"> <img src="1024px-Uber_logo_2018.svg.png" width="250"> </p>

## Context 
Uber is a ride-sharing application that started as a service for people who couldn't afford a taxi. It operates now in about 70 countries and 900 cities, and it generates over $14 billion revenue.

Uber's team found that sometimes drivers are not close enough when users need them. Uber's research shows that users accept to wait for 5-7 minutes and tend to cancel their ride if the driver takes longer to arrive.

Therefore, Uber's data team would like their app to be able to recommend hot-zones in New York City where the drivies should be.


## Goals of the project
 - Create an algorithm to find hot-zones in New York City where the drivers should be. The hot-zones should at least be described per day of the week.
 - Visualise the results on a map

I chose to concentrated on data from April 2014 for performance reasons but the approach can be applied to other periods covered by the dataset in analogous manner.

## Project files

The project includes several files:

1. Exploratory data analysis and finding pickup hot-zones with DBScan clustering algorithm

        1_uber_dbscan.ipynb

2. Finding pickup hot-zones with KMeans clustering algorithm (EDA is identical to the previous file)

        2_uber_kmeans.ipynb

3. Comparison of recommended driver positions found using the two clustering algorithms

        3_dbscan_vs_kmeans_comparison.ipynb

The project folder also includes:
- .csv dataset with information on Uber pickups in New York City in April 2014 (if needed, other dataset files for the project can be downloades from the S3 bucket - see *References* section)
- .csv files with driver positions found using DBScan and KMeans algorithms.

 ## References
  
- [Full dataset on AWS S3 bucket](https://uber-28-02-2023.s3.eu-west-3.amazonaws.com/uber-trip-data.zip)

- [Uber pickups in New York City dataset on Kaggle](https://www.kaggle.com/datasets/fivethirtyeight/uber-pickups-in-new-york-city)

- [Being a Uber driver in NYC requires a special license](https://www.uber.com/us/en/drive/requirements/fast-lane/#:~:text=Unlike%20in%20other%20cities%2C%20you,road%20to%20higher%20earnings%20today)
