Introduction:-  Most of product based companies and industrial sector use many machine for their day to day work.
As Machines do lot of machanical  work they are more prone to failures.  And failure to machine can cause lot of problem and reduction in production.
   one appraoch to deal with that problem is predicting which machine like to fail given sensor data,historical records 
and environmental data.
Here i used deep learning approach to predict which machine componenet is likly to fail.
file:
data: this folder contains raw data like maintenance history,sensor data,last componenet failure,machine model,age of machine etc.
model.h5 is trained model using raw data and tensorflow
data_processing contains code for preprocessing of data, removing outliers and hot encoding
