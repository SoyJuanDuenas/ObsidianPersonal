#inferential_statistics 

To understand what is sample and sampling distributions we will describe how can we obtain this distributions.

Let's say that we have a population of interest and we take a random sample from it, and based on that sample we calculate a sample statistic for example the mean of that sample. Then we repeat that process again and again, each one of the samples will have the own distributions which we call sample distributions, each observation in these distributions is a randomly sampled unit from the population, now the set of sample statistic also make a new distribution, where each observation isn't a unit from the population but a sample statistic.

![[Pasted image 20240506211742.png]]

The mean of the sampling distribution will probably be around the true population mean, and also the standard deviation of this sampling distribution will be probably much lower than the population standard deviation.

**The standard deviation of sampling distribution is called the Standard Error**

As the sample size of the sampling distribution increases, the standard error will decrease, this is related with the [[Central Limit Theorem]] that can be interpret in this context as:


> [!NOTE] Title
> The sampling distribution is nearly normal centered at the population mean with standard error equal to the population standard deviation divided by square root of the sample size.
> $$\overline{x} \sim N(\mu, \frac{\sigma}{\sqrt{n}})$$


Because $\sigma$ (population standard deviation) is often unknow we use $S$, the standard sample deviation to estimate the standard error. With this in mind we can say that as the sample size increases we would expect samples to yield more [[consistent]].


### References

To develop this chunk we will use the next one online course as our main source

- YouTube https://www.youtube.com/playlist?list=PLc_ATubXG-SQiDUmQgsuiSficQ51Xbeaq
- Coursera Inferential Statistics - Duke University