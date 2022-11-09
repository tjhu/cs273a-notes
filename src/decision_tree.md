# Decision Tree

- virtually nested if-else statement
- works well with mix of features

## Training

- if leaf
  - predict the majority or the mean
- else
  - find the best split
  - split the data with the split
  - recurse

## Entropy

Measure of randomness

$ H(X) = \sum p(x) \log \frac{1}{p(x)} $

Information reduction
