# Hand-Gesture-Recognition-using-CNN-and-RNN
Gesture Recognition for Smart Televisions using Deep Learning Modeling Techniques
## Problem Statement
As a data scientist at a home electronics company which manufactures state of the art smart televisions, you want to develop a cool feature in the smart-TV that can recognise five different gestures performed by the user which will help users control the TV without using a remote.

The gestures are continuously monitored by the webcam mounted on the TV. Each gesture corresponds to a specific command:

- Thumbs up: Increase the volume
- Thumbs down: Decrease the volume
- Left swipe: Jump backwards 10 seconds
- Right swipe: Jump forward 10 seconds
- Stop: Pause the movie
Each video is a sequence of 30 frames (or images).

## Understanding the Dataset
The training data consists of a few hundred videos categorised into one of the five classes. Each video (typically 2-3 seconds long) is divided into a sequence of 30 frames(images). These videos have been recorded by various people performing one of the five gestures in front of a webcam - similar to what the smart TV will use.

The data is in a zip file. The zip file contains a train and a val folder with two CSV files for the two folders. These folders are in turn divided into subfolders where each subfolder represents a video of a particular gesture. Each subfolder, i.e. a video, contains 30 frames (or images). Note that all images in a particular video subfolder have the same dimensions but different videos may have different dimensions. Specifically, videos have two types of dimensions - either 360x360 or 120x160 (depending on the webcam used to record the videos). Hence, pre-processing is needed to standardise the videos.

Each row of the CSV file represents one video and contains three main pieces of information - the name of the subfolder containing the 30 images of the video, the name of the gesture and the numeric label (between 0-4) of the video.

## Goals of this Project
In this project, a model needs to be built to recognise 5 hand gestures. Our task is to train different models on the train folder to predict the action performed in each sequence or video and which performs well on the val folder as well. The final test folder for evaluation is withheld - final model's performance will be tested on the test set.

## This project consist of below files
A Jupyter Notebook consists of different models with multiple experiments and with the best model we get using MobileNet architecture (CNN-RNN Stack).
A .h5 file containing best model weights
A Write up which is containing detailed procedure followed in choosing the final model. The write up has been started with the reason for choosing the base model, then highlight the reasons and metrics taken into consideration to modify and experiment to arrive at the final model.
Link of the Dataset: https://drive.google.com/uc?id=1ehyrYBQ5rbQQe6yL4XbLWe3FMvuVUGiL
