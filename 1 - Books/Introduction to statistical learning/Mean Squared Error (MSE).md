
**Mean Squared Error (MSE)** measures the average squared difference between observed values and predictions, penalizing large errors more heavily than small ones. hence this is a error measure in the [[regression problem]]

Given true values $y_i$ and predictions $\hat{y}_i$  for $i=1,\dots,n$

$$
\text{MSE}=\frac{1}{n}\sum_{i=1}^n (y_i-\hat{y}_i)^2
$$
## Interpretation

- Units: **squared units** of $Y$ (e.g., if $Y$ is dollars, MSE is $dollars^2$).
- Lower is better.
- Strongly penalizes large errors → sensitive to outliers.

# visualization:

![[Pasted image 20260505174627.png]]


Usually we perform MSE out-sample data (test data), we are interested in the accuracy of the predictions that we obtain when we apply our method to previously unseen test data. We don’t really care how well our method predicts last week’s output. We instead care about how well it will predict tomorrow’s output or next month’s output.

This is important because allow us to avoid [[overfitting]] that could happen when we use a MSE in training data often with more flexible models.

## Relation to RMSE
$$
\text{RMSE}=\sqrt{\text{MSE}}
$$
[[Root Mean Square Error (RMSE)]] is in the **same units** as $Y$, often easier to interpret.




