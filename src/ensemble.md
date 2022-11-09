# Ensemble

- weighted average among several predictors
- stacked model: the one taking the average
- prefer using different data to train the stacked model

## Bagging

- short for bootstrap aggregation
- sample subset of the data and train one classifier each
- allow each decision tree to have high variance(overfitting)
- reduce overfitting since outliers are only seen by a few models
- lower variance with the same low bias

## Random Forest

- bagging but sample features instead of the data

## Gradient Boosting

- learn a bunch of weak underfit learners

## Ada Boost

- increase the weights of the data points that are correct and decrease the correct ones and train a new classifier
- combine all classifiers with their coefficients
- higher coefficient for learner with less error
