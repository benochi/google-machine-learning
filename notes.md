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
