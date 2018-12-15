# Yelp-User-Rating-Prediction-and-Restaurant-Recommendation
The repository contains all the required files and the data for performing User Rating Prediction and Restaurant Recommendation.

The file structure is as follows: User_Rating_Prediction_using_NLP_and_Restaurant_Recommendation - Copy.ipynb - This fle contains the code for User rating prediction and restaurant recommendation. The other details are explained in the notebook.

YELP_EDA.ipynb - This file contains the Exploratory Data Analysis performed on different datasets that can be found under the Yelp_data folder.

The data has been fetched from https://www.kaggle.com/yelp-dataset/yelp-dataset
Steps to process data:
1) Once you download the zip file, write the following commands to exactly get the amount of rows that have been used in this project.
2) Create a folder called yelp_data in the same directory as your other files which can be found above.
3) Extract all the files under yelp_data and while reading each file, make sure to add the nrows = 100000 parameter while reading individual files in Pandas Dataframe. So, the syntax would be:
import pandas as pd
review = pd.read_csv('yelp_data\\review.csv', nrows=100000)
In this project we have taken in review_reduced and other reduced files which are nothing but just comma separated value files with 100000 rows. Hence, the change in name of the file.

Yelp_data folder - Contains different files in the form of comma separated values for business, reviews, checkin, tip, photos and users.

app.py - Contains the code which invokes a flask application where the user can enter any text in the text box in the form of a review to get a possible prediction based on natural language processing performed on the text entered.
For running this file, you need to have flask installed. If you don't have it installed, you can do pip import flask or python -m pip install flask from command line. Once flask is installed, you can open your terminal and write the command
python app.py which would give you a localhost IP address. Copy that IP address on your browser and hit enter. You will get redirected to a web page which would allow you to enter text into a box followed with a predict button. Once you hit the predict button, wait for sometime as the model gets trained for predicting the possible user review which he/she will give to the restaurant based on his/her reviews.
