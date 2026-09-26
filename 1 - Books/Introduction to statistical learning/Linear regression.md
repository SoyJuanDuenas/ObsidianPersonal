**Linear regression** is a simple [[parametric method]] used in [[Supervised statistical learning]]. It is especially useful for [[regression problem|regression problems]], where the goal is to predict a quantitative response. Linear regression can be divided into two main types: simple linear regression and multiple linear regression.

# Simple Linear Regression

**Simple Linear Regression** assumes that there is an approximately linear relationship between a predictor $X$ and a response variable $Y$. This relationship can be expressed as:

$$
Y \approx \beta_0 + \beta_1 X
$$

where:

- $\beta_0$ is the intercept. It represents the [[expected value]] of $Y$ when $X=0$.
- $\beta_1$ is the slope. It represents the expected change in $Y$ associated with a one-unit increase in $X$.

Since $\beta_0$ and $\beta_1$ are unknown [[parameter|parameters]], we need to [[estimate]] them using the training data. The estimation can be done using a [[estimator]], the three fundamental estimation frameworks in statistics and econometrics are: 

- [[Ordinary least squares (OLS)]]
- [[Maximum Likelihood Estimation (MLE)]]
- [[Generalized Method of Moments (GMM)]]

The estimated regression line is:

$$
\hat{Y}
=
\hat{\beta}_0
+
\hat{\beta}_1 X
$$

where:

- $\hat{Y}$ is the predicted value of $Y$.
- $\hat{\beta}_0$ is the estimated intercept.
- $\hat{\beta}_1$ is the estimated slope.

For each observation $i$, the prediction is:

$$
\hat{y}_i
=
\hat{\beta}_0
+
\hat{\beta}_1 x_i
$$

The difference between the observed value $y_i$ and the predicted value $\hat{y}_i$ is called the residual:

$$
e_i
=
y_i
-
\hat{y}_i
$$

In this setting, $\beta_0$ and $\beta_1$ are the true but unknown population [[parameters]], while $\hat{\beta}_0$ and $\hat{\beta}_1$ are their sample estimates.