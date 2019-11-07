---
layout: post
title:      " LSTM neural network"
date:       2019-11-07 22:37:14 +0000
permalink:  lstm_neural_network
---


Long Short Term Memory neural networks or LSTMs are a subset of recurring neural networks with the added specialty of being able to forget about the past so to speak. As the layers of the neural network are transversed the input from layers of the distant past have less of affect on the input into the current neurons compared to more recent layers.Another way to think of functionality of a LSTM is to picture the normal input gate and output gate plus a forget gate in each node of the network. 
There are several ways for LSTMs to train their data through loss functions which include categorical cross-entropy, binary cross-entropy and mean square error.If the loss function could be thought of as the experiment being done, the optimizer are considered the equipment being utilized. The most popular optimizer is Adam which is hybrid of the Adapative Gradient Algorithm and Root Mean Square Propagation.
When building an LSTM model there are three major components that will affect the duration of computation including, the number of hidden layers, the batch size and how many epochs are listed. Using the Keras library allows for multiple iterations through LSTM neural networks in series.The batch size is the number of inputs going into the model which need to be transposed into an array containing the rows, time-series, and columns.
The epochs will determine how many times your data will be trained and tested. When  a loss function reaches its a local minium the rate of learning is beginning to slow down as well however if the number of epochs is continued there can be overfitting of the training data. If training data is repeatedly iterated the accuracy of training data will increase yet when given that testing sets being a quarter of the size of training sets will score much lower accuracies due to their smaller size. Similar to other aspects of LSTMs there are options when considering how to output final values using sigmoidal or softmax and hyperbolic tangential functions.
