Introduction:-  Most of product based companies and industrial sector use many machine for their day to day work.
As Machines do lot of machanical  work they are more prone to failures.  And failure to machine can cause lot of problem and reduction in production.
   one appraoch to deal with that problem is predicting which machine like to fail given sensor data,historical records 
and environmental data.
Here i used deep learning approach to predict which machine componenet is likly to fail.
files:
data: this folder contains raw data like maintenance history,sensor data,last componenet failure,machine model,age of machine etc.
model.h5 is trained model using raw data and tensorflow
data_processing contains code for preprocessing of data, removing outliers and hot encoding
model contains code used to devlop and train the model.
prediction and evluation contains code for evaluating and prediction using trained model

dependencies:
Numpy
Pandas
scikit_learn
tensorflow
python
dataset:Dataset is taken from microsoft azure predictive maintenanace
Context
It consists of the following data:

Machine conditions and usage: The operating conditions of a machine e.g. data collected from sensors.
Failure history: The failure history of a machine or component within the machine.
Maintenance history: The repair history of a machine, e.g. error codes, previous maintenance activities or component replacements.
Machine features: The features of a machine, e.g. engine size, make and model, location.
Details
Telemetry Time Series Data (PdM_telemetry.csv): It consists of hourly average of voltage, rotation, pressure, vibration collected from 100 machines for the year 2015.

Error (PdM_errors.csv): These are errors encountered by the machines while in operating condition. Since, these errors don't shut down the machines, these are not considered as failures. The error date and times are rounded to the closest hour since the telemetry data is collected at an hourly rate.

Maintenance (PdM_maint.csv): If a component of a machine is replaced, that is captured as a record in this table. Components are replaced under two situations: 1. During the regular scheduled visit, the technician replaced it (Proactive Maintenance) 2. A component breaks down and then the technician does an unscheduled maintenance to replace the component (Reactive Maintenance). This is considered as a failure and corresponding data is captured under Failures. Maintenance data has both 2014 and 2015 records. This data is rounded to the closest hour since the telemetry data is collected at an hourly rate.

Failures (PdM_failures.csv): Each record represents replacement of a component due to failure. This data is a subset of Maintenance data. This data is rounded to the closest hour since the telemetry data is collected at an hourly rate.

Model Evaluation: for model evaluation metrices like precision,recall,f1_score and confusion matrix are being used.
Result: model show extraordinary capabilites over training and test data set
got accuaracy 0.98 ,precision 0.975,recall 0.984 and f1_score 0.974(all these value are over scale o to 1)
Author:krishan
credit:kaggle for providing dataset

future devlopment :i am trying integrate model over web and make it suitable for easy to use for non tech background too and i am researching about feedback loop so soon this model have ability to take  realtime feedback

