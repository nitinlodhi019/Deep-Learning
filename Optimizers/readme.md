# Optimizer

In deep learning, an optimizer is a crucial element that fine-tunes a neural network's parameters during training. Its primary role is to minimize the model's error or loss function, enhancing performance.

**Types of optimizers:**

1 . *Stochastic gradient descent (SGD):*

A simple and effective algorithm that updates the weights for each training example individually 

2 . *Gradient descent:* 

An iterative algorithm that moves towards the minimum value of a function 

3 . *RMSprop:*

An adaptive learning rate algorithm that divides the learning rate by a moving average of the squared gradients

4 . *Adadelta:*

An algorithm that adapts the learning rate of each parameter during training 

5 . *Adagrad:* 

An algorithm that uses an adaptive learning rate per parameter 

**Optimizer considerations**

*Learning rate:* 

A high learning rate can cause the algorithm to overshoot the minimum, while a low learning rate can make convergence slow

*Data scaling:* 

The performance can degrade if the data is not scaled properly
