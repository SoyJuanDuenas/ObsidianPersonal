
The mathematical expression of bias is the follow:

$$
bias(\hat\theta) = E[\hat\theta] - \theta 
$$
Where:

- $\theta$ is the true parameter
- $\hat\theta$ is the [[estimator]]
- $E[\hat\theta]$ is the [[expected value]] of the [[estimator]] / average [[estimator]] value across repeated samples.

since $\hat\theta$ is a [[random variable]] we can visualize the bias as:

![[Pasted image 20260505231041.png]]


In a applied approach, Bias refers to the error that is introduced by [[estimate]] a real-life problem, which may be complicated for a any model. For example a [[linear regression]] assumes that there is a linear relationship between $Y$ and $X_1,X_2,...,X_p$. This is unlikely because any real-life problem usually don't have such a simple linear relationship, so performing [[linear regression]] will undoubtedly result in some bias in the [[estimate]] of $f$.