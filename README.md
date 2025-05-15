# Assignment 03 - Course Optimization of Business Processes

The file actuals.csv contains historical volume of 1456 days of a call center. 
This data is simplified: each year has 52 weeks, thus it is exactly 4 years of data.
It contains no events, but trend, intra-year and intra-week seasonality.

Write a python program for which the output are the answers to the following questions:
a (3p). Use linear regression to make a forecasting model for the daily volumes. Note that the trend is non-linear, thus try different (polynomial?) trends. Use a test set of 10 weeks, and report on the WAPE, and make a forecast for week 260.
b (1.5p). Implement the stationary distribution of the Erlang A model in python such that, for given parameters, you can compute the minimal number of agents required to make sure that the delay probability is below a certain level.
c (1p). Use this to obtain the required number of agents during the days of week 260 assuming that the volume is equally distributed, using a 60/0 SL, an AHT of 5 minutes, an average patience of 10 minutes, and 14 opening hours. Compute the total number of agent hours.
d (0.5p). Do the same, but now assuming that the volume increases linearly (stepwise from quarter to quarter) from 0 to twice the average.
e (3p). There are 2 types of shifts for a week: 4 times 6 hours or 3 times 8 hours, always on consecutive days. E.g., Mon-Wed 8 hours per day, or Thu-Sun 6 hours per day. Implement an ILO problem that determines the optimal combination of shifts such that the minimal number of hours is scheduled and the required number of hours per day is met. Calculate the shift inefficiency: (scheduled - required) / required.

Submit both python code and a pdf with the answers. Grading is purely based on the usage of the required methods and the correctness of the answers.