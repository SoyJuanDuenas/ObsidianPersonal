#probability 

The **Total Probability Theorem** is a fundamental rule in probability theory that relates marginal probabilities to [[conditional probability]]. It states that if $\{B_1, B_2, \ldots, B_n\}$ is a [[partition of the sample space]] $\Omega$, then for any event $A$:

$$P(A) = \sum_{i=1}^{n} P(A \mid B_i) P(B_i)$$
# Explanation

- **Partition of $\Omega$**: The set $\{B_1, B_2, \ldots, B_n\}$ is a [[partition of the sample space]] $\Omega$ if these events are mutually exclusive and collectively exhaustive, meaning:
	- $B_I \neq \emptyset$
    - $B_i \cap B_j = \emptyset$ for all $i \neq j$
    - $\bigcup_{i=1}^{n} B_i = \Omega$
- **Conditional Probability**: $P(A \mid B_i)$ is the probability of event $A$ given that $B_i$​ has occurred.

### Example

Consider a medical test for a disease that has the following probabilities:

- $P(D)$: Probability of having the disease
- $P(\neg D)$: Probability of not having the disease
- $P(T \mid D)$: Probability of a positive test given the presence of the disease
- $P(T \mid \neg D)$: Probability of a positive test given the absence of the disease

Using the Total Probability Theorem, the probability of testing positive $P(T)$ can be calculated as:

$$P(T) = P(T \mid D) P(D) + P(T \mid \neg D) P(\neg D)$$
### Applications

- **Medical Testing**: Determining the overall probability of a positive test.
- **Risk Management**: Assessing the total probability of different risk factors contributing to a loss.
- **Reliability Engineering**: Calculating the probability of system failure based on the probabilities of individual component failures.