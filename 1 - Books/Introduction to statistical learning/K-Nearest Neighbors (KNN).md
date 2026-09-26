
**k-Nearest Neighbors (KNN)** is a [[non-parametric method]] used to [[estimate]] an outcome for a point $x_0$ based on the outcomes of the $K$ most similar training observations to $x_0$, according to a chosen distance metric.

Given a positive integer $K$ and a test observation $x_0$, the KNN classifier first identifies the $K$ points in the training data that are closest to $x_0$. These points are represented by $\mathcal{N}_0$. KNN then estimates the [[conditional probability]] for class $j$ as the fraction of points in $\mathcal{N}_0$ whose response value equals $j$:

$$
\widehat{Pr}(Y = j \mid X = x_0)
=
\hat{p}_j(x_0)
=
\frac{1}{K}
\sum_{i \in \mathcal{N}_0}
I(y_i = j)
$$

Using the logic of the [[Bayes classifier]], KNN classifies the test observation $x_0$ into the class with the largest estimated conditional probability:

$$
\hat{y}(x_0)
=
\arg\max_{j}
\left(
\frac{1}{K}
\sum_{i \in \mathcal{N}_0}
I(y_i = j)
\right)
$$

The choice of the [[hyperparameter]] $K$ determines the flexibility of the model. According to [[The Bias-Variance Trade-Off]], increasing $K$ generally increases [[bias]] and reduces [[variance]], while decreasing $K$ generally reduces bias and increases variance.


