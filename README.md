# real-estate-price-prediction-project
In terms of project architechture first we are going to take a home price dataset from kaggle.com which is for bangalore city in india and will use that to build our ML model. It will include concepts like data cleaning, feature engineering, dimesionality reduction, outlier removel, etc. Once the model will built then we will export it into a pickle file and then will write a python flask server which can consume this pickle file and do price prediction for you. This python flask server will export HTTP endpoints for various requests and the UI written in HTML, CSS and Java Script will make http get and post calls. In terms of tools and technology we will use python as a programming language, pandas for data cleaning, Matplotlib for data visualisation, SK-learn for model building, Python flask for a backend server, HTML,CSS and Java Scripr for our website.

steps involved;
--download the dataset from https://www.kaggle.com/datasets/amitabhajoy/bengaluru-house-price-data
--data cleaning 
