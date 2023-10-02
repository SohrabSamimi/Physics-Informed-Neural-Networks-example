# Physics-Informed-Neural-Networks-example

We use the Pytorch DL library to write the code.

We first train a baseline Neural Network to learn the Cosine function.

The Train Loss is around 1e-5 and the Test Loss is around 0.04 after 2000 epochs.

![Baseline_NN_cosine](https://github.com/SohrabSamimi/Physics-Informed-Neural-Networks-example/assets/58103877/8e6d8f5b-0f7d-417c-9f96-f455f8145983)

Afterwards, we see the Cosine function as the solution of a second order differential equation,

and we use Physics-Informed Neural Networks to learn it using only 15 data points on an interval of length 7.

We see that the PINNs prediction and the true Cosine agree very well.


