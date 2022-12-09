# real-estate-price-prediction-project

In terms of project architechture first we are going to take a home price dataset from kaggle.com which is for bangalore city in india and will use that to build our ML model. It will include concepts like data cleaning, feature engineering, dimesionality reduction, outlier removel, etc. In terms of tools and technology we will use python as a programming language, pandas for data cleaning, Matplotlib for data visualisation, SK-learn for model building.

steps involved;
--download the dataset from https://www.kaggle.com/datasets/amitabhajoy/bengaluru-house-price-data
--data cleaning 
Removed some not_so_important columns 
Removed records where null was there
Some other anomalies also corrected
--feature engineering
We made a new column price_per_sqft
--dimensionality reduction 
There were 1304 unique locations i.e. too  many . Locations which had only one or two data points are converted  to "other" to make it simple and effective.
--outlier removal
We removed records where area per room is <300sqft
We removed records where price per sqft was <(m-sd) and >(m+sd)
       where m=mean and sd=standard deviation.
We removed records where no. of bathrooms>(bedrooms+2)
--Then we converted the location(categotical) into a numeric column as ML model not interprets text data by using one hot encoding ie also called dummmies.
--model building
then we made a linear regression model which had a accuracy of 81.15%
