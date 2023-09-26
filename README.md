# Physics-Informed-Neural-Networks-example

We use the Pytorch DL library to write the code.

We first train a Neural Network to learn the Cosine function. We generate our data by working on interval [0 ; 2$pi$] that we discretize uniformly using 200 points.

We then split this data in Training Set(80%) and Test Set(20%).

We use Tanh and LeakyReLU as activation functions.

The Train Loss is around 1e-5 and the Test Loss is around 0.04 after 2000 epochs.

We notice that the model performs well on the training data but does not generalize well on the test set.

We show here under the curve of the cosine function and the curve of the evaluation of the learned model: we see that on the training set the two curve almost exactly agree, but not on the test set.
