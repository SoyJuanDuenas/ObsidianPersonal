#probability 

A **partition** of a [[sample space]] $\Omega$ in probability theory is a collection of collectively exhaustive and [[mutually exclusive events]]. These events cover all possible outcomes in the [[sample space]] without overlapping.

Let $\{B_1, B_2, \ldots, B_n\}$ be a partition of the sample space $\Omega$ if:

- $B_i \neq \emptyset$
- $B_i \cap B_j = \emptyset \text{ ,} \forall$  $i \neq j$ (mutually exclusive)
- $\bigcup_{i=1}^{n} B_i = \Omega$ (collectively exhaustive)

# Properties

**Mutually Exclusive**: No two events $B_i$​ and $B_j$​ in the partition can occur simultaneously.

$$B_i \cap B_j = \emptyset \quad \text{for all } i \neq j$$
**Collectively Exhaustive**: The union of all events in the partition covers the entire sample space.
$$\bigcup_{i=1}^{n} B_i = \Omega$$
# Formula aplication

Given a partition $\{B_1, B_2, \ldots, B_n\}$ of $\Omega$, for any event $A$ in $\Omega$, we can express $A$ in terms of the partition:

$$P(A) = \sum_{i=1}^{n} P(A \cap B_i)$$

# Example

Consider rolling a fair six-sided die. The sample space $\Omega$ is:

$$\Omega = \{1, 2, 3, 4, 5, 6\}$$
A possible partition of $\Omega$ can be:

$$B_1 = \{1, 2\}, \quad B_2 = \{3, 4\}, \quad B_3 = \{5, 6\}$$

These subsets $B_1, B_2, B_3$​ are mutually exclusive and collectively exhaustive.

### Importance in Probability

Partitions of the sample space are crucial for simplifying complex probability problems. They allow us to break down the problem into smaller, more manageable parts.

### Applications

- **[[Total Probability Theorem]]**: The theorem relies on partitioning the sample space to express the probability of an event as the sum of conditional probabilities.
- **[[Bayes' Theorem]]**: It uses partitions to relate conditional probabilities and update beliefs based on new evidence.
- **Decision Analysis**: Partitioning helps in evaluating different scenarios and their probabilities to make informed decisions.

