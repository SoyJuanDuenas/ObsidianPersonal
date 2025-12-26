#probability
A sequence of events is an ordered collection of events, usually indexed by the natural numbers. It can represent a series of events that occur in succession or are considered in a specific order.
# Formal Definition

A sequence of events is a list $\{A_n\}$ where each $A_n$​ is an [[event]] in the sample space $\Omega$, indexed by $n = 1, 2, 3, \ldots$ then

$$\{A_n\} = [A_1, A_2, \dots , A_n]  $$

## Non-Decreasing Sequence of Events

A sequence of events $\{A_n\}$ is non-decreasing if each event is a subset of the subsequent event:

$$A_1 \subseteq A_2 \subseteq A_3 \subseteq \cdots \subseteq A_n$$
In other words, each event includes all the outcomes of the previous event plus possibly additional outcomes, a visual representation by Venn Diagrams of this statement are the following figure.



![[Pasted image 20240723194358.png]]

## Example

Consider the experiment of flipping a coin indefinitely. Let $A_n$​ be the event that at least one head appears in the first $n$ flips. The sequence $\{A_n\}$ is non-decreasing because:

$$A_1 \subseteq A_2 \subseteq A_3 \subseteq \cdots \subseteq A_n$$

since if a head appears within the first $n$ flips, it will also appear within the first $n+1$ flips.

# Non-Increasing Sequence of Events

A sequence of events $\{B_n\}$ is non-increasing if each event is a superset of the subsequent event:

$$B_1 \supseteq B_2 \supseteq B_3 \supseteq \cdots \supseteq B_n$$

In other words, each event contains all the outcomes of the subsequent event and possibly more. A visual representation by Venn Diagrams of this statement are the following figure.

![[Pasted image 20240723202345.png]]

## Example

Consider the same coin flipping experiment. Let $B_n$​ be the event that no heads appear in the first $n$ flips. The sequence $\{B_n\}$ is non-increasing because:

$$B_1 \supseteq B_2 \supseteq B_3 \supseteq \cdots \supseteq B_n$$

Since if no heads appear in the first $n+1$ flips, then no heads appear in the first $n$ flips.

# Applications

Understanding sequences of events, including non-decreasing and non-increasing sequences, is essential in various applications such as:

- **[[Convergence in Probability]]**: Analyzing the convergence of sequences of [[random variable]]s.
- **Measure Theory**: Working with measures and integrals in advanced probability theory.
- **Stochastic Processes**: Studying the behavior of processes over time.
# Key Points

- A sequence of events is an ordered collection of events indexed by natural numbers.
- A non-decreasing sequence of events has each event as a subset of the next, while a non-increasing sequence has each event as a superset of the next.
- These concepts are foundational in understanding the limiting behavior of probabilities and in various applications in probability theory and statistics.