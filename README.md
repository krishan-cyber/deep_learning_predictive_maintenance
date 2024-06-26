Predictive Maintenance using Deep Learning

Introduction:-

Many product-based companies and industrial sectors heavily rely on machinery for their operations. However, machines are prone to failures due to mechanical wear and tear, which can lead to production disruptions and losses. Predictive maintenance aims to mitigate these risks by forecasting potential failures of machine components using sensor data, historical records, and environmental factors. This project employs a deep learning approach to predict which machine components are likely to fail, thereby enabling proactive maintenance strategies.

Files Included


data/: Contains raw data including maintenance history, sensor readings, previous component failures, machine models, and age.


model.h5: Trained TensorFlow model saved after training on raw data.


data_processing/: Code for data preprocessing, outlier removal, and one-hot encoding.


model/: Code used for developing and training the predictive maintenance model.


prediction and evaluation/: Code for model evaluation and making predictions using the trained model.


Dependencies


Ensure you have the following dependencies installed to run the project:

Python 3.x<br>
Numpy<br>
Pandas<br>
scikit-learn<br>
TensorFlow<br>


Dataset<br>
The dataset used in this project is sourced from Microsoft Azure Predictive Maintenance, consisting of the following data:<br>

Telemetry Time Series Data (PdM_telemetry.csv): Hourly averages of voltage, rotation, pressure, and vibration collected from 100 machines during 2015.


Error (PdM_errors.csv): Errors encountered by machines during operation, not resulting in shutdowns.


Maintenance (PdM_maint.csv): Records of proactive and reactive maintenance activities, including component replacements.


Failures (PdM_failures.csv): Records of component replacements due to failures.


Methodology


Data Preprocessing


The raw data underwent preprocessing, including outlier removal and one-hot encoding of categorical variables.

Model Development


The model was developed using a deep learning approach with various hidden layers and appropriate activation functions.


Model Evaluation


Evaluation metrics such as precision, recall, F1-score, and confusion matrix were used to assess the model's performance.

Results


The model achieved high accuracy (0.98), precision (0.975), recall (0.984), and F1-score (0.974) on both training and test datasets.


Author: Krishan<br>
Credits: Kaggle for providing the dataset<br>


Future Developments

Integrated model over web to make it suitable for easy to use for non tech background too<br>


Soon this model have ability to take  Realtime feedback
