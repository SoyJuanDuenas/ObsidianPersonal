
Is possible to show that the [[expected value]] of the test [[Mean Squared Error (MSE)]], for a given value $x_0$, can always be decomposed into the sum of three fundamental quantities: the [[variance]] of $\hat{f}(x_0)$, the squared [[bias]] of $\hat{f}(x_0)$ and the [[variance]] of the error term $\epsilon$ ([[irreducible error]])

$$
\mathbb{E}\!\left( y_0 - \hat{f}(x_0) \right)^2
= \operatorname{Var}\!\left(\hat{f}(x_0)\right)
+ \left[\operatorname{Bias}\!\left(\hat{f}(x_0)\right)\right]^2
+ \operatorname{Var}(\varepsilon).
$$

This equation tell us to that in order to minimize the expected test error, we need to select a [[statistical learning]] method that simultaneously achieves low [[variance]] and low [[bias]]. 

Note that [[variance]] is inherently a nonnegative quantity, and squared [[bias]] is also nonnegative. Hence, we see that the [[expected value]] of test MSE can never lie below $Var(\epsilon)$ that is the [[irreducible error]].

# The trade off core

As a general rule, as we use more flexible methods, the [[variance]] will increase and the [[bias]] will decrease. The relative rate of change of these two quantities determines whether the of the test [[Mean Squared Error (MSE)]] increases or decreases.

this could be explained by the fitting capacity of the models, more flexible models mean that they will have more sensibility to the train data, meaning better fitting, now if you have a model which is too sensible to the training data, you will have [[overfitting]].

due $\hat f (x_0)$ is a [[estimator]] for $f(x_0)$, then $\hat f (x_0)$ is a [[random variable]] because it's a function of the sample data, then $var(\hat f (x_0))$ measure how sensible are my [[estimator]] to the sample data.

# A simulation

In order to understand better this trade off we're going to perform a brief simulation.

Let be $y = sin(x) + \epsilon$ the true generation function $f(x)$

Then we try to [[estimate]] / fit the following models:

- linear regression
- polynomial degree 2
- degree 5
- degree 10
- degree 20

As we can see in the following figure the linear regression are far away of the true function, but we find a sweet spot in degree 5 regression, now from this point we begin to see that the model begins to diverge form the true function due to [[overfitting]]. 

![[bias_variance_dark.png]]

``` r
set.seed(123)

# -----------------------------
# 1. Generate training data
# -----------------------------

n <- 40

x <- runif(n, 0, 2*pi)

y_true <- sin(x)

y <- y_true + rnorm(n, sd = 0.3)

train <- data.frame(x, y)

# -----------------------------
# 2. Generate test grid
# -----------------------------

x_test <- seq(0, 2*pi, length.out = 500)

y_test_true <- sin(x_test)

test <- data.frame(x = x_test)

# -----------------------------
# 3. Fit models with different flexibility
# -----------------------------

degrees <- c(1, 2, 5, 10, 20)

par(mfrow = c(2,3))

results <- data.frame()

for(d in degrees){

  # Fit polynomial regression
  model <- lm(y ~ poly(x, d, raw = TRUE), data = train)

  # Predictions
  pred_train <- predict(model, newdata = train)
  pred_test  <- predict(model, newdata = test)

  # Compute MSE
  train_mse <- mean((train$y - pred_train)^2)

  test_mse <- mean((y_test_true - pred_test)^2)

  results <- rbind(results,
                   data.frame(
                     degree = d,
                     train_mse = train_mse,
                     test_mse = test_mse
                   ))

  # -----------------------------
  # Plot
  # -----------------------------

  plot(train$x, train$y,
       main = paste("Degree =", d),
       pch = 19,
       xlab = "x",
       ylab = "y")

  # True function
  lines(x_test, y_test_true,
        lwd = 2,
        lty = 2)

  # Fitted function
  lines(x_test, pred_test,
        lwd = 2)
}

print(results)
```

# Mathematical Proof of Bias-Variance Trade-Off

Suppose the true data-generating process is

$$
Y_0 = f(x_0) + \varepsilon,
$$
with
$$
E[\varepsilon] = 0,
\qquad
Var(\varepsilon)=E[\varepsilon^2]=\sigma^2.
$$

We want to analyze the expected prediction error at the point $x_0$:

$$
E\left[(Y_0-\hat f(x_0))^2\right].
$$
Substituting the true model:
$$
E\left[(Y_0-\hat f(x_0))^2\right]
=
E\left[(f(x_0)+\varepsilon-\hat f(x_0))^2\right].
$$
Add and subtract $E[\hat f(x_0)]$ inside the square:
$$
=
E\left[
\left(
f(x_0)-E[\hat f(x_0)]
+
E[\hat f(x_0)]-\hat f(x_0)
+
\varepsilon
\right)^2
\right].
$$
Define
$$
a=f(x_0)-E[\hat f(x_0)],
$$
$$
b=E[\hat f(x_0)]-\hat f(x_0),
$$
$$
c=\varepsilon.
$$
Then:
$$
E[(a+b+c)^2].
$$
Expanding the square:
$$
(a+b+c)^2
=
a^2+b^2+c^2+2ab+2ac+2bc.
$$

Taking expectations:

$$
E[(a+b+c)^2]
=
E[a^2]
+
E[b^2]
+
E[c^2]
+
2E[ab]
+
2E[ac]
+
2E[bc].
$$

Now evaluate each term.

Since $a$ is constant:
$$
E[a^2]
=
(f(x_0)-E[\hat f(x_0)])^2.
$$
The second term is the variance of the estimator:

$$
E[b^2]
=
E[(\hat f(x_0)-E[\hat f(x_0)])^2].
$$
The third term is:

$$
E[c^2]
=
E[\varepsilon^2].
$$
Now analyze the cross terms.

First:

$$
E[ab]
=
aE[b].
$$

But

$$
E[b]
=
E[E[\hat f(x_0)]-\hat f(x_0)]
=
0.
$$

Hence:

$$
E[ab]=0.
$$

Similarly:

$$
E[ac]
=
aE[\varepsilon]
=
0.
$$

Finally, assuming $\varepsilon$ is independent of $\hat f(x_0)$:

$$
E[bc]
=
E[b]E[\varepsilon]
=
0.
$$

Therefore all cross terms vanish, leaving

$$
E[(Y_0-\hat f(x_0))^2]
=
(f(x_0)-E[\hat f(x_0)])^2
+
E[(\hat f(x_0)-E[\hat f(x_0)])^2]
+
E[\varepsilon^2].
$$

Thus,

$$
\boxed{
E[(Y_0-\hat f(x_0))^2]
=
Bias(\hat f(x_0))^2
+
Var(\hat f(x_0))
+
Var(\varepsilon)
}
$$

where

$$
Bias(\hat f(x_0))
=
E[\hat f(x_0)]-f(x_0),
$$

and

$$
Var(\hat f(x_0))
=
E[(\hat f(x_0)-E[\hat f(x_0)])^2].
$$

$$
\mathbb{E}\!\left( y_0 - \hat{f}(x_0) \right)^2
= \operatorname{Var}\!\left(\hat{f}(x_0)\right)
+ \left[\operatorname{Bias}\!\left(\hat{f}(x_0)\right)\right]^2
+ \operatorname{Var}(\varepsilon).
$$