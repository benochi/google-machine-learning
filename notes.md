Notes from Google Machine Learning

Supervised machine learning

example: a particular instance of data -

Labeled example: has {features, label}: (x, y) - used to train model, the y is the thing we're predicting(price of a commodity, etc)

Unlabeled example: has {features, ? }: (x, ?) - Used for making predications on new data.

Model: maps examples o predicted labels: y' -Thing that does the learning.

LOSS:

x/y line = y = w,x, + b
Loss will show how well our line is doing at predicting an example. compare prediction to actual value.

L2 Loss = squared error - square of difference between prediction and label = (observation - prediction)^2 = (y-y)^2
x = house square footage, y = housing price(trying to predict y)

L2Loss = E(y- prediction(x))^2

(x,y) EpsilonD

Epsilon: we're summing over all examples in the training set

D: sometimes useful to average over all examples, so divide by D

Linear regression: y = mx+b (m is slope of the line, b is the y-intercept)

in machine learning = y(predicted label) = b + w1x1(1 is the weight of feature 1), b is the bias (the y-intercept), sometimes referred to as w0.
x1 is a known input

more sop[histicated models have more weights, IE y1=b + w1x1 + w2x2 +w3x3

Training and loss:

In supervised learning, a machine learning algorithm builds a model by examining many examples and attempting to find a model that minimizes loss; this process is called **empirical risk minimization**.

Loss is the penalty for a bad prediction. That is, **loss** is a number indicating how bad the model's prediction was on a single example. If the model's prediction is perfect, the loss is zero; otherwise, the loss is greater. The goal of training a model is to find a set of weights and biases that have _low_ loss, on average, across all examples. For example, Figure 3 shows a high loss model on the left and a low loss model on the right. Note the following about the figure:

**Mean square error** ( **MSE** ) is the average squared loss per example over the whole dataset. To calculate MSE, sum up all the squared losses for individual examples and then divide by the number of examples:

mse= 1/n E(y-prediction(x))^2 E=(x,y)epsilonD

where:

- (x,y) is an example in which
  - x is the set of features (for example, chirps/minute, age, gender) that the model uses to make predictions.
  - y is the example's label (for example, temperature).
- prediction(x) is a function of the weights and bias in combination with the set of features x.
- D is a data set containing many labeled examples, which are (x,y) pairs.
- N is the number of examples in D.

Although MSE is commonly-used in machine learning, it is neither the only practical loss function nor the best loss function for all circumstances.
