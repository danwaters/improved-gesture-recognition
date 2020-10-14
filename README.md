# P2: Improved Gesture Recognition
Improved gesture recognition project for CSCE 5280 @ UNT

Contributors: TabashumThasina, Wise61, arifahmed420, danwaters

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

![Confusion matrix](https://github.com/danwaters/improved-gesture-recognition/blob/main/Images/confusion-matrix.png)



