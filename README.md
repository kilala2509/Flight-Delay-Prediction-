# Flight-Delay-Prediction-
Flight arrival time prediction is a critical aspect of the aviation industry, as delays and cancellations can result in significant financial losses for airlines and passengers. An accurate prediction model allows airlines and airports to plan and manage flight operations effectively. In addition to negatively affecting an airline's income and customer satisfaction, delays and cancellations can be inconvenient for passengers, resulting in missed connections, scheduling difficulties, and other travel-related problems

# Description
In this project, we aim to predict flight arrival time from four major US airports to Syracuse, New York using a machine learning model. The model should take into account various factors that can impact arrival times, including weather conditions, airport operations, and other external factors. The primary goal of this project is to improve the accuracy and reliability of flight arrival time predictions, which can have a significant impact on airlines' revenue and customer satisfaction, as well as passengers' travel experience. By providing accurate and reliable predictions, airlines and airports can better plan and manage their operations, reducing delays and cancellations and improving overall efficiency.

# Dependencies

 Python
 Jupyter Notebook
 Pandas
 Numpy
 
# Methodology

In this scenario, we are going to predict the arrival of flights. We will be predicting whether a given flight is Early, On time, Late, or Severely late. This is a classification problem.

We will be training a classifier model using flight and weather data for a period of one year and then will use the trained model to predict the flight arrival for the given two weeks
 
# Data set

The first step in data collection for this project was identifying the appropriate data sources. We used The Bureau of Transportation Statistics (BTS), to collect flight data. The flight dataset contains flights from airports from January 1, 2022, to December 31, 2022. Four departure files were downloaded, one from each of the four airports - Chicago O'Hare (ORD), Denver International (DEN), Newark Liberty (EWR), and Washington Dulles (IAD) and then one arrival file for Syracuse Hancock International Airport.

In order to make predictions more accurate, we have also used factors like weather data that can cause airline delays.
The data was extracted from 'https://www.visualcrossing.com/weather-data'.


# Model Selection

	CatBoost Classifier

CatBoost provided some level of interpretability. It could output feature importance scores, which helped us understand which features are most relevant for the prediction. As shown in the graph below, this classifier gave more importance to weather conditions unlike random forest model that prioritized flight number over other factors. In summary, CatBoost, being a powerful gradient boosting framework, that could handle categorical features, missing values, and overfitting. It was fast, scalable, and provided some level of interpretability.

Model score: 0.43 
![image](https://github.com/kilala2509/Flight-Delay-Prediction-/assets/46477646/875f7538-0828-4900-92da-1a1fb2e316f2)

