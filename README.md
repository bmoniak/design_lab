# Hello World! Hello JetBot!

## General description of the project:

The main feature of this project is the hand recognition function. It allows the robot to recognize the hand gestures, like hand pointing left or right, or OK sign. To recognize the gestures it uses the Alexnet network retrained for our specific purposes using transfer learning. For the project we used Jupyter notebooks, and it is possible to run the whole code on the jetson nano platform, even the retraining of the neural network.<br>
The Jetson that we are using is a version with 4 gb of ram, and it wouldn’t be possible to run the tasks on the version with 2 gb of ram. Jetson is placed in a 3D printed platform, and in this configuration it is also called Jetbot. There are two motors connected to the wheels, a powerbank used to power both the motors and the jetson, WiFi module, and camera. The version of the OS installed on the SD card in Jetson is Jetpack 4.3, and Jetbot version 0.4.0.

## Contents:
There are a total of three Jupyter notebooks, each one of them serving different purposes. 
- **Data_Collection.ipynb** - in this notebook we are collecting the photos required to retrain the neural network.
- **Train_Model.ipynb** - In this notebook we are retraining the Alexnet neural network. We are replacing the top layer with the labels that we have created, and we train it to recognize those patterns. 
- **Gesture_Recognition.ipynb** - In this notebook we are using the retrained model to demonstrate how the network works. 
- *best_model.pth - unfortunately the trained model is too big to upload on github as the maximum file size is 100 MB. In case you'd like to access the file please contact us - we will sort something out :)*

## Authors: 
Adrian Smoła
Bartłomiej Moniak
