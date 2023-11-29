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

In supervised learning, a machine learning algorithm builds a model by examining many examples and attempting to find a model that minimizes loss; this process is called **empirical risk minimization** .
