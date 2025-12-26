#probability

Independent events are a fundamental concept in probability theory. Two or more events are considered independent if the occurrence of one [[event]] does not influence the occurrence of the other events. In other words, knowing the outcome of one [[event]] provides no information about the outcome of the other events.

It's important to remember than independent events are different than [[mutually exclusive events]] by definition

### Formal Definition:

For two events $A$ and $B$ in a [[probability space]], $A$ and $B$ are independent if and only if: $$P(A \cap B) = P(A) \times P(B)$$
Where:

- $P(A \cap B)$ represents the probability that both events $A$ and $B$ occur simultaneously.
- $P(A)$ is the probability of [[event]] $A$ occurring.
- $P(B)$ is the probability of [[event]] $B$ occurring.

This is equivalent to say

- $P(A \mid B) = P(A) \text{  , } P(B) > 0$
- $P(B \mid A) = P(B) \text{  , } P(A) > 0$

This relationship can be extended to more than two events.

$$P \left( \bigcap_{i = 1}^{n} A_i\right) = \prod_{i=1}^{n}P(A_i)$$

### Conditional Independence:

Two events $A$ and $B$ are conditionally independent given a third [[event]] $C$ if: $$P(A \cap B | C) = P(A | C) \times P(B | C)$$
This means that given the occurrence of $C$, the occurrence of $A$ does not affect the occurrence of $B$ and vice versa.
## Properties of Independent Events

- **Symmetry:** If $A$ and $B$ are independent, then $B$ is independent of $A$.
- **Complement Independence:** If $A$ and $B$ are independent, then $A^c$ (the complement of $A$) and $B$ are also independent.