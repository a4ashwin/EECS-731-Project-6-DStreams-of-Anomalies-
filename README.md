# Assignment-Project-6-
 5th assignment of EECS 731 Intro to Data Science -  D(St)reams of Anomalies

 Prerequisites
 Python 3.7.3, Jupyter Notebook, Pandas Library, Numpy Library & sklearn Library

 Introduction:
 In this project, we are going to transform the dataset of NYC Taxis by using feature engineering. We are going to modify the dataset into a new dataset that has the meaningful data to fit Anomaly detection model so we can detect anomalies and deal with them in the future. We have 2 features- timestamp and value. timestamp is the time and date of a particular day and value represents the number of taxis hire in NYC in that half hour.

 Idea:
 We need to detect the anomalies in data in this project so that the we can get an idea about how the outliers in the data. We will be doing our analysis on the basis of per day hires of taxi. To do that, first we will split the timestamp to get dates and total number of taxis hired on that day. Then, we will fit the IsolationForest Anomaly detection model with the features and then test the anomalies.

 Process:
 - Download the data from https://github.com/numenta/NAB/tree/master/data
 - Load the dataset into Pandas dataframe from nyc_taxi.csv
 - Split the timestamp in to Time and Date columns
 - Drop the columns that are not significant in predicting the demand of the products.
 - Drop the rows with Nan(missing values) as they won't help in achieving our goal and also, they will create discrepancies in prediction.
 - Get the sum of hired taxi for each day.
 - Initialize and fit the IsolationForest model.
 - Calculate the RMSE value and plot the predicted demand with the actual demand.

 Result:
 We have successfully used the exploratory data analysis technique to get the idea of the data and remove insignificant data from the original dataset. We have used feature engineering to transform and make a final meaningful dataset for our particular goal. We successfully implemented IsolationForest Anomaly detection model to detect anomalies in the data. We have got 3 anmalies with keeping the Contamination value to 0.01.

 Built With:
 Jupyter Notebook
 Python 3.7.3
 Pandas
 NumPy

 Authors:
 Ashwin Rathore

 License:
 This project is created for Course EECS 731 Assignment for University of Kansas.

 Acknowledgments:
 https://github.com/numenta/NAB/tree/master/data
