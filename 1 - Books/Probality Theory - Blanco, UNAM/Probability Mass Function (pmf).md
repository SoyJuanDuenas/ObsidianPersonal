#probability
# Definition

A Probability Mass Function (PMF) is a [[Probability function]] that gives the probability that a discrete [[random variable]] is exactly equal to some value. It provides the probabilities of all possible values of a discrete [[random variable]].

# Properties

1. **Non-negativity**: $$p(x) \geq 0 \text{ ,} \forall x $$
2. **Normalization**: The sum of the probabilities for all possible values of the discrete [[random variable]] is 1, which can be expressed as: $$\sum_{x} p(x) = 1$$
3. **Probability Calculation**: The probability that the [[random variable]] $X$ takes a specific value $x$ is given directly by the PMF: $$P(X=x)=p(x)$$
# Examples

- **Binomial Distribution**: The PMF of a binomial distribution with parameters $n$ (number of trials) and $p$ (probability of success) is: $$p(x) = \binom{n}{x} p^x (1 - p)^{n - x} \quad \text{for } x = 0, 1, 2, \ldots, n$$where $\binom{n}{x}$ is the binomial coefficient.

- **Poisson Distribution**: The PMF of a Poisson distribution with rate parameter $\lambda$ is: $$p(x) = \frac{\lambda^x e^{-\lambda}}{x!} \quad \text{for } x = 0, 1, 2, \ldots$$
### Visualization

A PMF is typically visualized as a bar graph. The x-axis represents the possible values of the [[random variable]], and the y-axis represents the probability of each value. Each bar's height corresponds to the probability of that specific value.

### Applications

PMFs are used in various fields such as computer science, economics, and genetics to model and analyze situations where outcomes are discrete. They help in understanding the distribution and behavior of discrete data and in making probabilistic predictions.

### Key Points

- The PMF provides a complete description of the probability distribution of a discrete [[random variable]].
- The PMF gives the exact probability of each possible value that the [[random variable]] can take.

