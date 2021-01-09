# activityPrediction

Activity Prediction is a technique where video or movement sensor data is used to classify the activity of a subject
into one of many classes such as: walking, sleeping or eating. In this project, data from a set containing
3 Million readings from an IMU (Inertial Measurement Unit) which monitored the Angular Velocity & Acceleration of a given Cow in the X, Y & Z axes.

This dataset presented numerous challenges such as non-fixed time frequency of readings and very imbalanced classes. Subsequently, the infrequency of sample times was addressed by calculating the mean measurements for every second of time elapsed; allowing for predictions to be made within this fixed time-period. Since for this project, I wanted to optimise the F1-Score, the class weights were balanced in order to prevent the classification model from neglecting the lesser-represented classes in the set.

I then trained a Random Forest on the features described and was able to report training F1-Score of 83%.
