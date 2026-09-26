
The mathematical expression of variance or also called **the second moment around the mean**  is the follow:

$$
var(X) = E[X - E[X]^2]
$$
Where

- X is a [[random variable]]
- $E[X]$ is the [[expected value]] of a [[random variable]]   

We can visualize the variance of a discrete [[random variable]] as the following figure:

![[Pasted image 20260506105533.png]]



This intuition led us to conclude that the variance measure how much a random variable fluctuates around its expected value.

Now, the variance is given in square units, so to interpretate better the result we can add a square root, this measure is called the [[standard deviation]].  

## Variance in statistical learning 

Variance refers to the amount by which $\hat{f}$ would change if we [[estimate]] it using a different training data set. Since the training data are used to fit the [[statistical learning]] method, different training data sets will result in a different $\hat{f}$. But ideally the [[estimate]] for $f$ should not vary too much between training sets. However, if a method has high variance then small changes in the training data can result in large changes in $\hat{f}$.