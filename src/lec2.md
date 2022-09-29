# Lecture 2

## Nearest neighbor

* An exampler-based model.
* Find the nearest existing data point and output its $y$.
* Piece-wise linear boundaries(TODO: figure).
* Perfect memorization of the training data.

### Problem

* When the number of dimensions increases, we need more data to fill in the space.
* "almost all" data are equally far away.
* Could be very slow.

### K-Nearest Neighbor

* Predict the average of the K-nearest neighbors instead of just one.
* Much smoother than the Nearest Neighbor.
* Still piecewise linear boundaries.
* More noise tolerant.

### Weighted K-Nearest Neighbor

* Can be weighted by the distance. It becomes 1-NN if $\alpha$ is too big.
* Can have clever distance function to make some features more important than the others.

## Linear Regression

* Prediction with linear response: $\hat{y} = \theta \cdot x^T$

* Find a cost function $J$ then we can learn.
* Mean Square Error(MSE): easiest error function.

### Gradient Descent

* To find the best $\theta$ to minize the loss, we can visualize the error doing the isocontour plot(TODO: figure).
* Find the gradient and go the opposite way and we will head towards the direction of the smallest loss.
