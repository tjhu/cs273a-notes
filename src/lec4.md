# Lecture 4

## Perceptron Classifier

- take a linear response and turn it into a class decision
- $f(x;\theta)$ = class decision
- AKA a linear classifier

## Separability

- a data set is separable by a learner if there's an instance of the learner that can seperate the data (TODO: figure)
- adding features or just a more complex classifier might separate them(TODO: figure)

## Feature representations

- 1-of-K encoding: make each enum value its own feature
  - prone to overfitting due to the increase in number of features

## Perceptron learning

Linear regression problems:

## Gradient learning classifier

The MSE in linear response are too sensitive to points away from the regression line even if the prediction is correct.

We wrap a smooth function like sigmoid or logistic function around it that doesn't penalize "point-away-from-line" we we can gradient descent.

A good surrogate loss penalize data points close to the decision boundary even if it's on the right side.

Negative log likely hood is very smooth.


## Logostic Regression

- model $\sigma(\theta X^T)$ as a probability
- just another loss function like MSE
- the regularization term wo

## Multi-class linear classifiers

- one classifier per class
- during training, we update the $\theta$ for just the class with the highest response