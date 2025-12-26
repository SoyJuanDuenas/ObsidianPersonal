#econometrics 

A Panel data is a set of data where we have a group of observations in two or more time moments for a initial approach we will explain this with two observations and then we will generalize.

# Two time periods data panel

The two time periods of the data panel doesn't have to be contiguous, it can be for example $t = 1982$ and $t + 1 = 1987$, well now we can discompose the error in two parts a $a_{i}$ **error component constant in the time** and a $u_{it}$**error component variable in the time**

Then we have the following formula:

$$y_{it} + \beta_0 + \delta_0d2 + \beta_1x_{it} + a_{i} + u_{it}$$
where $t = 1, 2$

## Estimation by pooled

A first approach is estimate $\beta_1$ just joining the time periods and estimate by[[Ordinary least squares (OLS)]] this is called Pooled OLS.

$$y_{it} + \beta_0 + \delta_0d2 + \beta_1x_{it} + v_{it}$$
Where $v_{it} = a_i + u_{it}$

With this approach we should suppose than:

$$E[a_{i} | x_{it}] = 0 $$
$$E[u_{it} | x_{it}] = 0$$
If this are false we have a bias by [[Heteroskedasticity]], additional of this suppose, we are not using the properties and opportunities than give us the panel data (control by $a_i$) 

## Estimation by first difference

Using the panel properties we can eliminate the error component constant in the time differentiating the two periods, let's see the algebra:

$$y_{i1} = \beta_0 + \beta_1x_{i1} + a_{i} + u_{i1}$$
$$y_{i2} = (\beta_0 + \lambda_0 ) + \beta_1x_{i2} + a_{i} + u_{i2}$$


$$y_{i2} - y_{i1} = (\beta_0 + \lambda_0 ) - \lambda_0 + \beta_1x_{i2} - \beta_1x_{i1} + a_{i} - a_{i} + u_{i2} - u_{i1}$$
$$y_{i2} - y_{i1} = \delta_0 + \beta_1(x_{i2} - x_{i1}) + u_{i2} - u_{i1}$$
$$\Delta y_{i} = \delta_0 + \beta_1 \Delta x_{i} + \Delta u_{ii}$$

This equation is called First-differenced equation, and can be estimated by the usual [[Ordinary least squares (OLS)]] it's important to remember than the model should keep the following suppose:
$$E[\Delta u_{i} | \Delta x_{i}] = 0 $$
And also there should be some variability in $\Delta x_{it}$ this fails when $x_{it}$ is constant in the time for all individuals (gender) or when the rate of change is the same for all observations (age) 

Then when we estimate the $\beta_1$ we called it First difference estimator, it's important to remember than the differentiation reduce the variation between explicative variables, because it just capture the differentiation in time, no between individuals.

For this we have a variance between and a variance within, the variance between are how in a cross - section the individuals change and the variance within are how a individual change in time.

# Multiperiod Data panel

We can use data panel in more than two periods, this is called Fixed Effects general model.
$$y_{ti} = \delta_1 + \sum_{j=2}^{T} \delta_j(dj_t) + \sum_{k=1}^{K} \beta_k x_{i+k} + a_{i} + u_{it}$$
If $a_i$ are correlated with at least one of the regressors, then we have a bias in [[Ordinary least squares (OLS)]] estimators, for this we can use first differences in multiperiod data panel.

When we differentiate and apply first differences in a multiperiod data panel we have the following model:

$$\Delta y_{ti} = \delta_0 + \sum_{j=3}^{T} \delta_j(dj_t) + \sum_{k=1}^{K} \beta_k \Delta x_{i+k} + a_{i} + \Delta u_{it}$$
we should assume than $\Delta u_{it}$ aren't autocorrelated in the time to be able to use standard errors and statistical test.





