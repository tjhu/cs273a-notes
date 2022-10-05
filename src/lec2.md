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
* Multiple ways to speed up the convergence
  * Big-small steps
  * Momentum
    * Keep going in the current momentum's direction
  * Second order method such as Newton's method
    * fast
    * expensive when the number of dimensions is high

#### Stochastic/online gradient descent(SGD)

One random data point, instead of all data points, at a time.

Benefits:

* more update per pass
* computationally faster

Draw back:

* no longer strictly descent
* don't know when to terminate

#### Batched SGD

A batch of data at a time to provide a good balance between GD and SGD.

### Algribic solver

* MSE can be solved algebricly(TODO: add equation)
* When the number of data is big, it could be very expensive.


### Outliers

MSE is very sensitive to outliers.

#### L1 error

Mean Absolute Error
