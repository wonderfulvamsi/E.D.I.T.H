# E.D.I.T.H
E.I.D.T.H is an AI which uses computer vision to predict the maximum speed limit dynamically, based on various parameters like number of vehicles &amp; their relative speeds.

The model was trained on an autonomous car's dataset.

# About the Dataset
Dataset is available here :
http://www.dbehavior.net/

![alt text](https://github.com/wonderfulvamsi/E.D.I.T.H/blob/master/db.JPG)

# About the model
After converting all the 120 images of each video of the dataset into gray scale.
![alt text](https://github.com/wonderfulvamsi/E.D.I.T.H/blob/master/grayscale.JPG)

The model was trained on 6000 samples of 50 sceans with 4 seconds duration each and tested on 1800 samples.

It achived 45% accuracy in predicting the original speed of the vechicle with only 0.9 loss(MSE).
![alt text](https://github.com/wonderfulvamsi/E.D.I.T.H/blob/master/graph.JPG)

The model had achived 66% accuracy in predicting the maximum speed limit.

# Model architecture
The model consists of a convolution(4), max pooling(4) & batch norm(2) layers.
Since a video is a sequential data, I've used a LSTM layer with 1200 nodes after the flatten layer.
