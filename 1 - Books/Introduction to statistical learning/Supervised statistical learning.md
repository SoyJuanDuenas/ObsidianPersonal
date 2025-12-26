
**Supervised learning** is the process of learning a function $\hat f$ that maps inputs $X$ to an output $Y$ from labeled examples $(x_i, y_i)$, aiming to **generalize** well to new, unseen data.

![[Pasted image 20251223101507.png]]



The objective is to choose a [[loss function]] $L(y,\hat y$) and learn $\hat f$ to minimize expected loss:

$$R(\hat f)=\mathbb{E}\left[L\big(Y,\hat f(X)\big)\right]$$
In practice we minimize empirical risk ([[training loss]]), often with [[regularization]]:
$$
\hat f = \arg\min_{f\in\mathcal{F}} \frac{1}{n}\sum_{i=1}^n L\big(y_i, f(x_i)\big) + \lambda\,\Omega(f)
$$

In this type of statistical learning we can find two different types of problems: first [[regression problem]] that is where $Y$ is continuous (e.g., price, yield, demand), for validate the performance of the model in this type of problems we can use common losses metrics as [[Mean Squared Error (MSE)]], [[Root Mean Square Error (RMSE)]] and [[MAE]] 

For another way, we can find the [[classification problem]] that happens when target $Y$ is categorical (e.g., fraud vs non-fraud),  for validate the performance of the model in this type of problems we can use common losses metrics as [[log loss]], [[accuracy]], [[F1]], [[AUC]].

Supervised learning is judged by **out-of-sample** performance: Train/validation/test split, [[Cross-Validation]] and another.

Usually we select the model family based on the nature of the dependent variable $Y$ the problem with this is some models works even if the dependent variable are numerical or categorical, with this in mind the typical model families in supervised statistical learning are:

- Linear models: [[linear regression]], [[Ridge]], [[Lasso]]
- Generalized linear models: [[logistic regression]] or [[Poisson regression]]
- Trees and ensembles: [[decision trees]], [[random forest]], [[gradient boosting]]
- Kernel methods: [[SVM]], [[kernel ridge]]
- Neural networks: [[MLPs]] and others deep models

## Connections
- [[Statistical Learning]]
- [[Prediction]]
- [[Inference]]
- [[Cross-Validation]]
- [[Regularization]]

## Minimal references
- James, Witten, Hastie, Tibshirani — *An Introduction to Statistical Learning*
- Hastie, Tibshirani, Friedman — *The Elements of Statistical Learning*

