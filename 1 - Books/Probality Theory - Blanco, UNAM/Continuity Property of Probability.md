#probability 
### Definition

The Continuity Property of Probability, also known as the Continuity Axiom, is a fundamental principle in probability theory that describes the behavior of the [[probability measure]] with respect to limits of [[sequences of events]]. It ensures that the [[probability measure]] is consistent with the limiting behavior of [[sequences of events]].

### Formal Statement

Let $\{A_n\}$ be a sequence of events such that $A_n \subseteq A_{n+1}$​ $\forall n$ (i.e., the sequence is non-decreasing). Then:

$$P\left(\bigcup_{n=1}^{\infty} A_n\right) = \lim_{n \to \infty} P(A_n)$$

Similarly, let $\{B_n\}$ be a sequence of events such that $B_n \supseteq B_{n+1}$ $\forall n$ (i.e., the sequence is non-increasing). Then:

$$P\left(\bigcap_{n=1}^{\infty} B_n\right) = \lim_{n \to \infty} P(B_n)$$

# Visual explain

![[Pasted image 20240726215745.png]]
![[Pasted image 20240726215302.png]]
### Examples

- **Non-Decreasing Sequence**: Suppose $A_n$ represents the [[event]] that at least one head appears in the first $n$ flips of a fair coin. As $n$ increases, the probability $P(A_n)$ increases and approaches 1. The continuity property ensures that: $$P\left(\bigcup_{n=1}^{\infty} A_n\right) = \lim_{n \to \infty} P(A_n) = 1$$
- **Non-Increasing Sequence**: Suppose $B_n$​ represents the [[event]] that no heads appear in the first $n$ flips of a fair coin. As n increases, the probability$P(B_n)$ decreases and approaches 0. The continuity property ensures that: $$P\left(\bigcap_{n=1}^{\infty} B_n\right) = \lim_{n \to \infty} P(B_n) = 0$$
### Visualization

The continuity property can be visualized using [[Probability Mass Function (pmf)]] or [[Cumulative Distribution Functions (cdf)]] where the behavior of probabilities over a sequence of events approaches a limit.

### Applications

The Continuity Property of Probability is used in various fields to ensure the consistency of probability measures with respect to limits. It is fundamental in:

- **Probability Theory**: For proving theorems and properties related to limits and convergence of events.
- **Statistical Inference**: In the analysis of large samples and asymptotic properties of estimators.
- **Stochastic Processes**: In understanding the behavior of processes over time, such as in [[Markov chains]] and [[random walks]].

### Key Points

- The Continuity Property of Probability ensures that the probability measure is consistent with the limiting behavior of sequences of events.
- For a non-decreasing sequence of events, the probability of their union equals the limit of their probabilities.
- For a non-increasing sequence of events, the probability of their intersection equals the limit of their probabilities.