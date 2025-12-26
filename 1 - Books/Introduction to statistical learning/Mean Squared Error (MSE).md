
**Mean Squared Error (MSE)** measures the average squared difference between observed values and predictions, penalizing large errors more heavily than small ones.

Given true values $y_i$ and predictions $\hat{y}$_i for $i=1,\dots,n$

$$
\text{MSE}=\frac{1}{n}\sum_{i=1}^n (y_i-\hat{y}_i)^2
$$
## Interpretation

- Units: **squared units** of $Y$ (e.g., if $Y$ is dollars, MSE is $dollars^2$).
- Lower is better.
- Strongly penalizes large errors → sensitive to outliers.

Usually we perform MSE out-sample data, we are interested in the accuracy of the predictions that we obtain when we apply our method to previously unseen test data. We don’t really care how well our method predicts last week’s output. We instead care about how well it will predict tomorrow’s output or next month’s output.

This is important because allow us to avoid [[overfitting]], when we use a MSE in training data, if we apply a more flexible and flexible model configurations, then the MSE will be lower, but if we use this in MSE test data, then could be high than expected.

Then is possible to show that the [[expected value]] of the test MSE, for a given value $x_0$, can always be decomposed into the sum of three fundamental quantities: the [[variance]] of $\hat{f}(x_0)$, the squared [[bias]] of $\hat{f}(x_0)$ and the [[variance]] of the error term $\epsilon$

$$
\mathbb{E}\!\left( y_0 - \hat{f}(x_0) \right)^2
= \operatorname{Var}\!\left(\hat{f}(x_0)\right)
+ \left[\operatorname{Bias}\!\left(\hat{f}(x_0)\right)\right]^2
+ \operatorname{Var}(\varepsilon).
$$

This equation tell us to that in order to minimize the expected test error, we need to select a [[statistical learning]] method that simultaneously achieves low [[variance]] and low [[bias]]. Note that [[variance]] is inherently a nonnegative quantity, and squared [[bias]] is also nonnegative. Hence, we see that the [[expected value]] of test MSE can never lie below $Var(\epsilon)$ that is the irreducible error.

As a general rule, as we use more flexible methods, the [[variance]] will increase and the [[bias]] will decrease. The relative rate of change of these two quantities determines whether the test MSE increases or decreases.

## Relation to RMSE
$$
\text{RMSE}=\sqrt{\text{MSE}}
$$
[[Root Mean Square Error (RMSE)]] is in the **same units** as $Y$, often easier to interpret.