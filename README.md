# Physics-Informed-Neural-Networks-example

We first train a baseline Neural Network to learn the Cosine function.

We see here under a very good performance on the train set but not on the test set:

![Baseline_NN_cosine](https://github.com/SohrabSamimi/Physics-Informed-Neural-Networks-example/assets/58103877/8e6d8f5b-0f7d-417c-9f96-f455f8145983)

Afterwards, we take a completely different approach and we see the Cosine function as the solution of a second order differential equation.

We use Physics-Informed Neural Networks to learn it using only 15 data points on an interval of length $7$.

We see that the $PINNs$ prediction and the true Cosine agree very well even outside the training set (15 points):

![PINNS_COSINE](https://github.com/SohrabSamimi/Physics-Informed-Neural-Networks-example/assets/58103877/3e3350aa-18dc-4e3a-9015-8e22306984fb)

After training the model, we have an average error of $5.10^{-6}$ on a test set of 500 points.

The PINNS technique not only allows to get a good estimation of the function itself but also of its derivatives

as we see below.

We recall that we should get  $NN'(x) = -sin(x)$ and $NN''(x) = -cos(x)$

![1st 2nd derivatives](https://github.com/SohrabSamimi/Physics-Informed-Neural-Networks-example/assets/58103877/8dd8f52c-50d1-4059-8c10-f79c621841fa)


This repository was inspired by the following article by Raissi et al. 2017 : https://arxiv.org/abs/1711.10561



