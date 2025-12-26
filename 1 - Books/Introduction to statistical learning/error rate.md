
**Error rate** is the proportion of observations that a classifier predicts incorrectly. A good classifier is one for which the test error is smallest

$$
\text{Error Rate}=\frac{1}{n}\sum_{i=1}^n I(y_i\neq \hat y_i)
$$

Here $\hat y_i$ is the predicted class label for the $i$ observation using $\hat f$. And $I(y_i\neq \hat y_i)$ is an indicator variable that equals $1$ if $y_i\neq \hat y_i$ and $0$ if $y_i = \hat y_i$ then the $i$ observation was classified correctly by our classification method; otherwise it was misclassified.

As in the regression setting, we are most interested in the error rates that result from applying our classifier to test observations that were not used in training. The test error rate associated with a set of test observations of the form $(x_0,y_0)$ is given by:

$$
Average(I(y_0= \hat y_0))
$$

It is possible to show that the test error rate is minimized, on average, by the [[Bayes classifier]], a very simple classifier that assigns each observation to the most likely class, given its predictor values. 