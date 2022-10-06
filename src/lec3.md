# Lecture 3

## Non-linear Regression

For n-th degree regression, we can just transform it by adding features with $x^2$, $x^3$, ..., $x^n$ and still be able to fit it as a linear regression.

## Bias & variance

- the higher the degree, the more overfitting it could be.
- higher order -> lower bias and higher variance.
- K-fold cross validation(split into K parts, use one as validation, do it K times, and take average) to pick a model to prevent overfitting.

## Regularization

- add the penalty for coefficient($L_2$ penalty) $\sum_i \theta^2_i$
- it makes the $\theta$ small and less prompted to overfitting.
- this also allows us to solve this algebraically because it's full rank.
- $L_p$ regularizer: $(\sum_i |\theta_i|^p)^\frac{1}{p}$. Large p prefer small non-zero params; small p prefer exact zeros.
