 #econometrics

A Pooled Cross Section is a set of data where we have a “[[time series]] of cross sections,” but the observations in each cross section do not necessarily refer to the same unit. ie, Randomly sampled [[cross sections]] of individuals at different points in time.

![[Pasted image 20240914112224.png]]

Because we are random sapling in each time period we can suppose that the observations sampled are independent. This mean than the error are not correlated with the error of another time periods.

# Benefits

- We can achieve a higher sample size
- find changes in distribution are easy, just add a [[dummy variable]] for each time period controlling by another variables.

It's important remember that with pooled cross sectional we cannot infer poblational conclusions. Usually we can find this type of data in surveys generated periodically like the GEIH in the Colombian context.

In the pooled cross section we should use dummy variables to differentiate the period base and the period to make the comparation.

# Example

We can perform a [[impact evaluation]] using pooled Cross Sections. We will use a Wooldridge example: the effect of Garbage Incinerator Location on House Values in North Andover MA

To perform this example let be 2 year pooled cross section of data for 1978 and 1981, the incinerator were built in 1981 and online in 1985, it's important to know that the project of the incinerator wasn't know in 1978

Then we will create a [[dummy variable]] *nearinc* where it takes the number 1 when the house is near the incinerator and 0 when isn't
$$rprice = \gamma_0 + \gamma_1nearinc + u$$
Then if the incinerator had a negative effect in the rental price of the house near the incinerator, then is expected $\gamma_1$ negative and statistically significant. Now is important to know if the incinerator are actually the cause of the change in the rental prices so in this cases the important focus are the changes in the $\gamma_1$ coefficient between 1978 and 1981 this type of estimator are called the [[Difference-in-difference]] estimator.

So, let





