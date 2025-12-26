#probability #bayesian_inference

Bayes' Theorem provides a way to update our beliefs about the probability of a hypothesis based on new evidence. This process is iterative, meaning that [[posterior]] probability from one round of evidence can become [[prior]] probability for the next round of evidence.

Bayes' Theorem is a fundamental theorem in probability theory that describes how to update the probabilities of hypotheses when evidence is given. It is named after the Reverend Thomas Bayes and is central to the field of Bayesian inference.

## The Formula

If $B_1, B_2, \dots$ are a [[partition of the sample space]] and $A$ are a [[event]] where $P(A) \neq \emptyset$, Then for each $j = 1,2,\dots$ Bayes' Theorem can be mathematically expressed as:

$$P(B_j \mid A) = \frac{P(A \mid B_j) \times P(B_j)}{\sum_{i = 1}^{\infty} P(A \mid B_i)\times P(B_i)}$$
# Proof

We start from [[conditional probability]], by definition:

$$P(B_j \mid A) = \frac{P(B_j \cap A)}{P(A)}$$
By the definition of [[conditional probability]] we can also express $P(B_j \mid A)$ as follows

$$P(B_j \mid A) = \frac{P(A \mid B_j) \times P(B_j)}{P(A)}$$
Using the definition of [[Total probability theorem]] and given $B_j$ are a [[partition of the sample space]] we can transform the denominator of the expression 

$$P(B_j \mid A) = \frac{P(A \mid B_j) \times P(B_j)}{\sum_{i = 1}^{\infty} P(A \mid B_i)\times P(B_i)}$$

## Example

### Problem Statement

Suppose we want to determine the probability that a person has a particular disease $B$ given that they have tested positive $T$ for it. Let:

- $P(B^+) = 0.01$ The prior probability of having the disease is 1%
- $P(T\mid B^+)$ = 0.99 The probability of testing positive if the person has the disease is 99%
- $P(T\mid B^-)$ = 0.05 The probability of testing positive if the person does not have the disease is 5%

### Solution

Applying the Bayes' Theorem to this problem give us the following formula:

$$P(B^+ \mid T) = \frac{P(T \mid B^+) \times P(B^+)}{(P(T \mid B^+)\times P(B^+)+(P(T \mid B^-)\times P(B^-))}$$

Replacing the given probabilities:

$$P(B^+ \mid T) = \frac{0.99(0.01)}{(0.99(0.01))+(0.05(0.99))} \approx 0.16 $$

So, the probability that the person has the disease given that they tested positive is approximately 16 %.

But, hoy can this be possible ? let's think in a sample of 1000 people one of that 1000 has the probability of suffer the disease and the test could identify it properly (the 99% of accuracy of the test if he person has the disease) but, what about the probability of testing positive if the person does not have the disease. In this case with a 5% of false positive means that there is another 5 people than will test positive but they doesn't has the disease, for that reason we will face with the probability to doesn't be the false positive in a sample of falses positives cases (1/6 = 0.16)

As we said in the beginning of this entry Bayes' Theorem are designed to be a iterative process meaning that [[posterior]] probability from one round of evidence can become [[prior]] probability for the next round of evidence.

This can be accomplished replacing the prior $P(B^+)$ probability for the result of $P(B^+ \mid T)$(posterior probability)

In the example means than after you take one test than give you a positive you will take a new and independent test, the updated probability will give you the probability that the person has the disease after obtain a second positive test.

$$P(B^+ \mid T) = \frac{0.99(0.16)}{(0.99(0.16))+(0.05(0.99))} \approx 0.76 $$
