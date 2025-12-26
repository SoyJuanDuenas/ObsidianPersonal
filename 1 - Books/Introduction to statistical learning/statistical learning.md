
Statistical learning refers to a vast set of tools for understanding data and their patterns. These tools can be classified as:

- [[Supervised statistical learning]]
- [[Unsupervised statistical learning]]

Statistical learning involves building a statistical model for make a [[prediction]] of a variable or a [[inference]], based on one or more inputs. the statistical model rely in probability theory under the assumption that the inputs has a relationship with the output or dependent variable.

This assumption can be formally expressed as:

$$
Y = f(X) + \epsilon
$$

However, the function $f$ that connects the input variable to the output variable is in general unknow, so building the statistical model we must [[estimate]] the $f$ function based on the observed points.

In essence, statistical learning refers to a set of approaches for estimating $f$. and evaluate the estimates obtained, this approaches can be characterized as either [[parametric method]] or [[non-parametric method]].

In the methods of statistical learning there is a trade off between interpretability and prediction accuracy, this mean that the choose of the model should be aligned to the objective.

In order to evaluate the performance of a statistical learning method on a given data set, we need some way to **measure how well its predictions actually match the observed data**. That is, we need to quantify the extent to which the predicted response value for a given observation is close to the true response value for that observation. In [[regression problem]] the most commonly-used measure is the [[Mean Squared Error (MSE)]] and for [[classification problem]] is the [[error rate]] that is the proportion of mistakes that are made if we apply our estimate $\hat{f}$ to the training observations: