# P2: Improved Gesture Recognition
Improved gesture recognition project for CSCE 5280 @ UNT

Contributors: TabashumThasina, Wise61, arifahmed420, danwaters

## Abstract
According to NIDCD, approximately 7 million people in the U.S. struggle and experience difficulty in using their voices1. Vocalization difficulty can lead to several social and daily life complications. With this in mind, our motivation is to use proper validation techniques as well as hypertune the parameters. 

We implemented GridSearch to better tune our model and improve the overall accuracy. We also implemented Group KFold Subject-Wise Cross Validation to our model to ensure it does not overfit, as well as to prove our model is not biased to the training data.

## Important Links
* [Notebook](https://github.com/danwaters/improved-gesture-recognition/blob/main/Notebooks/Improved%20Gesture.ipynb)
* [Notebook (pdf)](https://github.com/danwaters/improved-gesture-recognition/blob/main/Improved%20Gesture%20-%20Jupyter%20Notebook.pdf)
* [Training and validation data (csv)](https://github.com/danwaters/improved-gesture-recognition/blob/main/Data/gesture_data.csv) - CSV file including 133,136 samples with 6 subjects defined as user number 25-30 with 11 gestures. 

## Motivation
* According to NIDCD, more than seven million people have problems with speech.
* Difficulty with speech can lead to social and job related complications.
* By developing an assistive technology that allows the user to communicate more effectively, we can improve the daily life of the user.
* This project will help the user reduce the conversational response time and increase their ability to communicate more naturally.

## Group K-Fold Cross Validation
* For this project iteration we chose to implement subject-wise Group KFold Cross Validation.
* As our dataset consists of only six users, subject-wise will help to improve the overall accuracy when testing on a new user.
* We chose group kfold because it helps reduce bias between our training and test sets.

![TensorBoard](https://github.com/danwaters/improved-gesture-recognition/blob/main/Images/tensorboard.png)

## Subject-Wise Cross Validation Results
* After performing hypertuning and validation techniques, we were able to get an accuracy of approximately 97%.
* Some subjects had a higher accuracy than others, which is expected as different people will gesture in different manners. The standard deviation of accuray is 3.5%. 
* Note, except one subject showed around 90% accuary, but for others it was above 9
* We used confusion matrices to visualize this accuracy.


![Confusion matrix](https://github.com/danwaters/improved-gesture-recognition/blob/main/Images/confusion-matrix.png)

This confusion matrix is based on the 4th subject and shows a relatively high accuracy on predicting the gesture that the subject displayed. 

As we performed subject-wise cross validation, each subject has a correlated confusion matrix. Our model performed better on some user data, and worse on others.




