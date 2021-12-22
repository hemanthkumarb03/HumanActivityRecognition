# HumanActivityRecognition
 
This project is to build a Classical ML model on human engineered / hand crafted time series data and DL model(simple LSTM) on Raw time series data that predicts Human Activities such as Walking, Sitting, Laying, Standing, Walking_Upstairs, walking_Downstairs.


# Overview of Data:

The data is recorded with the help of sensors (accelerometer and Gyroscope) in that smartphone. 


Accelerometer and Gyroscope readings are taken from 30 volunteers(referred as subjects) while performing the following 6 Activities.

Walking
WalkingUpstairs
WalkingDownstairs
Standing
Sitting
Lying.

Readings are divided into a window of 2.56 seconds with 50% overlapping.

Accelerometer readings are divided into gravity acceleration and body acceleration readings, which has x,y and z components each.

Gyroscope readings are the measure of angular velocities which has x,y and z components.

Jerk signals are calculated for BodyAcceleration readings.

Fourier Transforms are made on the above time readings to obtain frequency readings.

Now, on all the base signal readings., mean, max, mad, sma, arcoefficient, engerybands,entropy etc., are calculated for each window.

We get a feature vector of 561 features and these features are given in the dataset.

Each window of readings is a datapoint of 561 features.

