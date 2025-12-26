#probability 

Let's say we some a [[random experiment]], by definition when we do a [[random experiment]] we don't know the output of the experiment, but in some cases we know which are the posibles outputs of the [[random experiment]]. In probability theory, the **sample space** (denoted by $\Omega$) is the set of all possible outcomes of a [[random experiment]].
# Notation

The sample space is typically denoted by the Greek letter $\Omega$.
## Example

Consider a simple experiment of flipping a coin. The sample space for this experiment is:

$$\Omega = \{ \text{Heads}, \text{Tails} \}$$
# Properties

- The sample space **$\Omega$** includes all possible outcomes.
- Each outcome in $\Omega$ is mutually exclusive and exhaustive.

# Usage in Probability

When calculating the probability of an [[event]], the event is considered as a subset of the sample space $\Omega$. For example, if we want to find the probability of getting Heads in a coin flip, we consider the subset $\{\text{Heads}\}$ of the sample space.

$$P(\text{Heads}) = \frac{\text{Number of favorable outcomes}}{\text{Total number of outcomes}} = \frac{1}{2}$$

# Types of Sample Spaces

1. **Discrete Sample Space**: Contains a finite or countably infinite number of outcomes.
    - Example: Rolling a die
    - $\Omega = \{1, 2, 3, 4, 5, 6\}$
2. **Continuous Sample Space**: Contains an uncountably infinite number of outcomes.
    - Example: Measuring the height of a person
    - $\Omega = \{x \in \mathbb{R} \mid x \geq 0\}$

