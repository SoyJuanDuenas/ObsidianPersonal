#probability

The probability axioms or also called Kolmogorov's Axioms are a set of three fundamental rules that any [[probability measure]] must satisfy. These axioms form the foundation of probability theory and ensure that probabilities are assigned consistently.
# The axioms

1. **Non-negativity**: The probability of any event AA is a non-negative number.
  $$P(A) \geq 0$$
2. **Normalization**: The probability of the [[sample space]] $S$ is 1. The sample space represents all possible outcomes of a [[random experiment]].

$$P(\Omega) = 1$$
3. **Additivity (or Sigma-additivity)**: For any countable [[sequences of events]] $A_1, A_2, A_3, \ldots$if events $A_1, A_2, A_3, \ldots$ are [[mutually exclusive events]], the probability of their union is the sum of their individual probabilities.

$$P\left(\bigcup_{i=1}^{\infty} A_i\right) = \sum_{i=1}^{\infty} P(A_i)$$
For every function which the Kolmogorov's Axioms are present we call it as [[Probability Measure]]. Using the Kolmogorov's Axioms and Set Theory we can obtain the following properties

# Derived Properties

From these axioms, several important properties and rules of probability can be derived:

1. **Complement Rule**: The probability of the complement of an event $A$ (i.e., the event that $A$ does not occur) is 1 minus the probability of $A$.$$P(A^c) = 1 - P(A)$$
2. **Probability of the Empty Set**: The probability of the empty set (an impossible event) is 0.

$$P(\emptyset) = 0$$
3. **Finite Additivity**: For any finite number of [[mutually exclusive events]] $A_1, A_2, \ldots,A_n$$$P\left(\bigcup_{i=1}^{n} A_i\right) = \sum_{i=1}^{n} P(A_i)$$
