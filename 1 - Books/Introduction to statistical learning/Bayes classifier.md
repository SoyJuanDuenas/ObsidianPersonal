
The **Bayes classifier** assigns each observation to the most likely class, given its predictor values. this is the optimal classifier for minimizing the test error rate on average and is defined as: 

$$P(Y=j\mid X=x_0)$$

So, Given classes $j \in \{1,\dots,J\}$, the predict function are defined as:

$$
\hat{y}(x)=\arg\max_{j} \; P(Y=j \mid X=x)
$$

The Bayes classifier produces the lowest possible test error rate called the Bayes error rate.

For a fixed value $X = x_0$​, the Bayes classifier chooses the most likely class. Therefore, its probability of being correct is:
$$
\max_{j} \; P(Y=j \mid X=x)
$$
Hence the probability of being wrong is:

$$
1 - \max_{j} \; P(Y=j \mid X=x)
$$
That is the Bayes error rate at $x_0$, to get the overall Bayes error rate, we average this error over all possible values of $X$:

$$
E_x[1 - \max_{j} \; P(Y=j \mid X=x)]
$$
$$
1 - E_x[\max_{j} \; P(Y=j \mid X=x)]
$$
The Bayes error rate is in this setting the equivalent of the [[irreducible error]]

This is classifier is in essence a [[conditional probability]]. But for real data we do not know the [[conditional distribution]] of $Y$ given $X$ meaning that computing the Bayes classifier is impossible.

Many approaches attempt to [[estimate]] the [[conditional distribution]] of $Y$ given $X$, and then classify a given observation to the class with highest estimated probability, a example is the [[K-Nearest Neighbors (KNN)]] method