#probability 

In probability theory, a probability space provides the formal mathematical framework for describing random experiments and the outcomes of these experiments. It is essential for defining probability measures and for the systematic study of random variables and events.

# Definition

A **probability space** is a triple $(\Omega, \mathcal{F}, P)$ where:

1. **[[Sample Space]] ($\Omega$)**: This is the set of all possible outcomes of a random experiment. Each element of $\Omega$ represents a distinct outcome.

2. **[[Sigma Algebra]] ($\mathcal{F}$)**: This is a collection of subsets of $\Omega$ that are considered "measurable." It is a [[sigma algebra]], meaning it is closed under countable unions, countable intersections, and complements. $\mathcal{F}$ contains all the events for which we want to define probabilities.

3. **[[Probability Measure]] ($P$)**: This is a function $P: \mathcal{F} \to [0, 1]$ that assigns a probability to each event in $\mathcal{F}$. The probability measure must satisfy the Probability axioms:

# Key Properties

1. **Sample Space ($\Omega$)**: Represents the full set of possible outcomes in a [[random experiment]] . For example, if we roll a fair die, $\Omega$ could be $\{1, 2, 3, 4, 5, 6\}$.

2. **Sigma Algebra ($\mathcal{F}$)**: Includes all subsets of $\Omega$ that we are interested in measuring. In a discrete probability space, $\mathcal{F}$ is often the [[power set]] of $\Omega$. In continuous spaces, $\mathcal{F}$ is usually a [[Borel Sigma Algebra]] or another appropriate [[sigma algebra]].

3. **Probability Measure (PPP)**: Assigns probabilities to the events in $\mathcal{F}$. The measure PPP must be consistent with the [[Probability axioms]], ensuring that the total probability is 1 and that probabilities are additive for [[mutually exclusive events]].

# Examples

**Discrete Probability Space**:

- **Sample Space**: $\Omega = \{1, 2, 3, 4, 5, 6\}$ (rolling a fair die).
- **Sigma Algebra**: $\mathcal{F}$ is the [[power set]] of $\Omega$, i.e., all subsets of $\Omega$.
- **Probability Measure**: $P(A) = \frac{|A|}{6}$ for $A \subseteq \Omega$, where $|A|$ is the number of the element in $A$.

**Continuous Probability Space**:

- **Sample Space**: $\Omega = [0, 1]$ (the interval of real numbers from 0 to 1).
- **Sigma Algebra**: $\mathcal{F}$ is the [[Borel Sigma Algebra]] on $[0, 1]$, which includes all intervals and more complex sets.
- **Probability Measure**: $P$ could be the uniform distribution where $P([a,b])=b−a$ for $0 \leq a \leq b \leq 1$.

 **Normal Distribution**:
  
- **Sample Space**: $\Omega = \mathbb{R}$ (all real numbers).
- **Sigma Algebra**: $\mathcal{F}$ is the [[Borel Sigma Algebra]] on $\mathbb{R}$.
- **Probability Measure**: $P$ is the normal distribution with mean $\mu$ and variance $\sigma^2$, where the [[Probability Density Function (pdf)]] is given by $f(x) = \frac{1}{\sqrt{2\pi\sigma^2}} e^{-\frac{(x - \mu)^2}{2\sigma^2}}$
