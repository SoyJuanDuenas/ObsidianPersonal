
# Handwriting summary:




# Why we want to estimate $f(x)$

This chapter begin with the fundamental equation of [[statistical learning]]

$$
Y = f(X) + \epsilon
$$
Where we assume that an output $Y$ is constructed by relationships with some other dependent variables and a error $\epsilon$ being the function $f()$ the relation ship and the $X$ the dependent variables.

If we try to understand the relationship among the independent variables and the dependent variable we will be in a [[inference]] problem but if we're more interested in a good estimate of the independent variable given the dependent variables we are going to be in the [[prediction]] problem.

The main problem here is estimate a proper $f()$ to have better predictions or to understand with accuracy the relationship between $X$ and $Y$ this mean find a function $\hat{f}()$ such that $Y \approx \hat{f}(X)$ for any observation $(X, Y)$ 

## How do we estimate $f(x)$

We use a subset of our data called training data to [[estimate]] $f(x)$ and we can use two different approaches using [[parametric method]] or [[non-parametric method]]

**Parametric methods** assume the data-generating process belongs to a family of distributions or functions (like a linear function) described by a **finite-dimensional [[parameter]] [[vector]]** $\theta \in \mathbb{R}^k$, and then [[estimate]] $\theta$ from train data.

Nonparametric methods [[estimate]] relationships or distributions **without assuming a fixed finite-dimensional parametric form**, allowing model complexity to adapt to the data, this mean that Non-parametric methods do not make explicit assumptions about the functional form of $f$ but have to [[estimate]] more parameters, meaning that is necessary to have more observations to address a proper estimation.

## Prediction Accuracy and Model Interpretability trade off

Following this idea interpretate models is more easy in simple models, for example in linear models, but linear models will not always fit into the proper $f(x)$ now, this is important in [[inference]] problems. In [[prediction]] problems we don't need to interpretate, just predict.

Which type of problem we want to answer are going to give us the type of model we should use a restrictive one or a flexible one.

## Types of statistical learning

[[Supervised statistical learning]] is the process of learning a function $\hat f$ that maps inputs $X$ to an output $Y$ from labeled examples $(x_i, y_i)$, aiming to **generalize** well to new, unseen data.

[[Unsupervised statistical learning]] is the set of methods that discover **structure** in data using only inputs $X$ but there is no labeled outcome $Y$, aiming to reveal patterns such as groups, low-dimensional representations, or latent factors.

Sometimes this question is not clear, for example if we have a set of n observation where $m < n$ we have both predictor measurement and response measurement but for the $n - m$ observations, we don't have response measurement this is a [[semi-supervised statistical learning]]
## Regression vs classification problems

[[regression problem]] is when $Y$ is continuous (e.g., price, yield, demand), for validate the performance of the model in this type of problems we can use common losses metrics as [[Mean Squared Error (MSE)]], [[Root Mean Square Error (RMSE)]] and [[Mean Absolute Error (MAE)]].

For another way, we can find the [[classification problem]] that happens when target $Y$ is categorical (e.g., fraud vs non-fraud),  for validate the performance of the model in this type of problems we can use common losses metrics as [[error rate]], [[Accuracy]], [[Precision]], [[Recall]], [[F1 Score]] or [[Confusion Matrix]]

# How do we know that we have a good model ?

On a particular data set, one specific model may work best, but some other method may work better on a similar but different data set. This mean that is an important task to decide for any given set of data which method produces the best result.




