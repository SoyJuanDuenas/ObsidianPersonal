
**Parametric methods** assume the data-generating process belongs to a family of distributions or functions described by a **finite-dimensional [[parameter]] vector** $\theta \in \mathbb{R}^k$, and then [[estimate]] $\theta$ from data.

This mean a two-step model-based approach:

- First, we make an assumption about the functional form. or shape, of $f$, in a [[linear regression]] the assumption is that $f$ is lineal in $X$.
$$f(X) = \beta_0 + \beta_1X_1 + \beta_2X_2 +\dots + \beta_pX_p$$
	This mean that instead [[estimate]] an entirely arbitrary p-dimensional function $f(X)$, one only needs to estimate the $p + 1$ [[coefficients]] $\beta_0, \beta_1 , \dots, \beta_p$

- After a model has been selected we perform a procedure that uses the training data to fit or train the model, In the case of the [[linear regression]] we wan to find values of these parameters such that:
$$Y \approx \beta_0 + \beta_1X_1 + \beta_2X_2 +\dots + \beta_pX_p$$
	the most common approach to fitting a linear regression is [[Ordinary least squares (OLS)]], however, OLS is one of many possible ways to fit the linear model.

The potential disadvantage of a parametric approach is that the model we choose will usually not match the true unknown form of $f$. If the chosen model is too far from the true $f$, then our [[estimate]] will be poor. We can try to address this problem by choosing flexible models that can fit many different possible functional forms for $f$. But in general, fitting a more flexible model requires estimating a greater number of parameters. These more complex models can lead to a phenomenon known as [[overfitting]] the data.