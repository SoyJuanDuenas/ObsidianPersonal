
The **Bayes classifier** solve [[classification problem]]s and is the *optimal* classification rule (under 0–1 loss) that assigns an input $x$ to the class with the **highest posterior probability**,  is the best possible classifier for a given data-generating process.

The Bayes classifier’s prediction is determined by the [[Bayes decision boundary]]
$$P(Y=j\mid X=x_0)$$

Note, that this is classifier is in essence a [[conditional probability]] 
Given classes $k \in \{1,\dots,K\}$, predict:
$$
\hat{y}(x)=\arg\max_{k} \; P(Y=k \mid X=x)
$$

This rule minimizes the **Bayes risk** (expected misclassification error) among all possible classifiers.
## Binary classification form
If $Y \in \{0,1\}$, the Bayes rule becomes:
$$
\hat{y}(x)=
\begin{cases}
1, & P(Y=1\mid X=x) > 0.5\\
0, & \text{otherwise}
\end{cases}
$$

## How to compute the posterior

By [[Bayes' Theorem]]:
$$
P(Y=k\mid X=x)=\frac{p(x\mid Y=k)\,P(Y=k)}{p(x)}
$$
with
$$
p(x)=\sum_{j=1}^K p(x\mid Y=j)\,P(Y=j)
$$

## Relation to “Bayesian classifiers” in practice

The Bayes classifier is an **ideal decision rule** that requires the true [[posterior distribution]] (unknown). Many approaches attempt to [[estimate]] the [[conditional distribution]] of $Y$ given $X$, and then classify a given observation to the class with highest estimated probability

- $p(x\mid y)$ and $P(y)$ (generative)
- or directly $P(y\mid x)$ (discriminative)

Examples:
- [[Naive Bayes]]: assumes conditional independence in $p(x\mid y)$
- [[LDA]]/[[QDA]]: assumes Gaussian class-conditional distributions
- [[Logistic regression]]: models $P(Y=1\mid X)$ directly (discriminative)

Another example could be [[K-Nearest Neighbors (KNN)]] that Given a positive integer $K$ and a test observation $x_0$, the [[K-Nearest Neighbors (KNN)]] classifier first identifies the $K$ points in the training data that are closest to $x_0$, represented by $\mathcal{N}_0$. It then estimates the [[conditional probability]] for class $j$ as the fraction of points in $\mathcal{N}_0$ whose response values equal $j$: