#probability
# Definition

A Probability Density Function (PDF) is a continuous [[Probability function]] that describes the relative likelihood of a continuous [[random variable]] to take on a given value. The PDF is non-negative everywhere, and the area under the curve of the PDF over the entire space is equal to 1, signifying total probability.

### Properties

1. **Non-negativity**: $$f(x) \geq 0 \text{ ,} \forall x$$ 
2. **Normalization**: The total area under the PDF curve is 1, which mathematically can be expressed as: $$\int_{-\infty}^{\infty} f(x) \, dx = 1$$
3. **Probability Calculation**: The probability that the [[random variable]] $X$ lies within a certain interval $[a, b]$ is given by the area under the PDF between $a$ and $b$: $$P(a \leq X \leq b) = \int_{a}^{b} f(x) \, dx$$
# Examples

- **Normal Distribution**: The PDF of a normal distribution with mean $\mu$ and standard deviation $\sigma$ is: $$f(x) = \frac{1}{\sqrt{2\pi\sigma^2}} \exp\left(-\frac{(x - \mu)^2}{2\sigma^2}\right)$$
- **Exponential Distribution**: The PDF of an exponential distribution with rate parameter $\lambda$ is: $$f(x) = \lambda e^{-\lambda x} \quad \text{for } x \geq 0$$

### Visualization

A PDF is typically visualized as a curve on a graph. The x-axis represents the values of the [[random variable]], and the y-axis represents the probability density. The area under the curve between any two points corresponds to the probability that the variable falls within that range.

### Applications

PDFs are widely used in various fields such as physics, engineering, finance, and social sciences to model and analyze real-world phenomena. They help in understanding the distribution and behavior of continuous data and in making probabilistic predictions.

### Key Points

- The PDF provides a complete description of the probability distribution of a continuous [[random variable]].
- While the PDF itself does not give the probability of the variable taking a specific value (since for continuous variables this probability is zero), it helps in determining the probability of the variable falling within a specified range.