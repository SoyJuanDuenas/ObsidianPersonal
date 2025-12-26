#probability 

Conditional probability measures the likelihood of an [[event]] occurring given that another [[event]] has already occurred. It helps in understanding how the probability of one [[event]] is affected by the occurrence of another [[event]], which is crucial for making informed decisions and predictions based on partial information.

### Definition

The conditional probability of an [[event]] $A$ given that another [[event]] $B$ has occurred is denoted by $P(A \mid B)$. It quantifies the probability of $A$ happening under the condition that $B$ is known to have occurred.

Formally, the conditional probability $P(A \mid B)$ is defined as:

$$P(A \mid B) = \frac{P(A \cap B)}{P(B)}$$

where:

- $P(A \cap B)$ is the joint probability that both events $A$ and $B$ occur.
- $P(B)$ is the probability that [[event]] $B$ occurs, and it must be greater than 0,  $P(B)>0$

# Explanation of the formula

When we talk about conditional probability we want to incorpore a new piece of information. In the following case the new piece of information $B$ already happen. Let's say there is two events $A$ and $B$, now if we say $B$ already happen that means for contradiction a outcome where $A$ happen but not $B$ is not possible. that statement can be formalized as $A \cap B$. This makes obvious the change of the denominator because we know $B$ already happen. Then the new [[sample space]] is $\Omega (B)$

Now it's just a matter of put the events in their probability.

# Examples

1. **Rolling a Die**:
    
    - **Scenario**: Consider rolling a fair six-sided die. Let $A$ be the event that the die shows a number greater than 4 (i.e., 5 or 6). Let $B$ be the event that the die shows an even number (i.e., 2, 4, or 6).
    - **Joint Probability**: The probability of rolling a 6 (the only number greater than 4 and even) is $(A \cap B) = \frac{1}{6}$​.
    - **Probability of B**: The probability of rolling an even number is $P(B) = \frac{3}{6} = \frac{1}{2}$
    - **Conditional Probability**: $P(A \mid B) = \frac{P(A \cap B)}{P(B)} = \frac{\frac{1}{6}}{\frac{1}{2}} = \frac{1}{3}$​ So, given that the die shows an even number, the probability that it is greater than 4 is $\frac{1}{3}$​.

1. **Medical Testing**:
    
    - **Scenario**: Suppose a certain medical test has a 95% chance of correctly identifying a disease (true positive) and a 5% chance of false positives. Let $A$ be the event that a patient has the disease, and $B$ be the event that the test is positive.
    - **Joint Probability**: If the disease prevalence is 1% in the population, the probability of both having the disease and testing positive needs to be calculated based on given rates.
    - **Conditional Probability**: The probability of having the disease given a positive test result can be computed using the conditional probability formula once you know $P(A \cap B)$and $P(B)$.

## special cases

If $A$ and $B$ are [[mutually exclusive events]] (also called [[disjoint sets]]) then by definition $A \cap B = \emptyset$ That is equivalent to $P(A \cap B) = 0$  