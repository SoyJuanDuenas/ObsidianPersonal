#probability 

In probability theory, an event is a set of outcomes of a [[random experiment]] to which a probability is assigned. Events are subsets of the [[sample space]], which is the set of all possible outcomes of the [[random experiment]].

# Formal Definition

An event $A$ is a subset of the [[sample space]] $\Omega$. If $\Omega$ is the [[sample space]] of a [[random experiment]], then $A \subseteq \Omega$.

## Types of Events

1. **Simple Event**: An event consisting of a single outcome. For example, rolling a 3 on a six-sided die.
2. **Compound Event**: An event consisting of more than one outcome. For example, rolling an even number on a six-sided die (which includes the outcomes 2, 4, and 6).
3. **Certain Event**: The event that contains all possible outcomes. It is the entire sample space $\Omega$. For example, in a coin toss, the event $\{heads, tails\}$.
4. **Impossible Event**: The event that contains no outcomes. It is the empty set $\emptyset$. For example, rolling a 7 on a six-sided die.

### Examples

- **Coin Toss**: In the experiment of tossing a fair coin, the sample space is $\Omega = \{\text{heads}, \text{tails}\}$. Possible events include:
    - $A = \{\text{heads}\}$: The event of getting heads.
    - $B = \{\text{tails}\}$: The event of getting tails.
- **Die Roll**: In the experiment of rolling a fair six-sided die, the sample space is $\Omega = \{1, 2, 3, 4, 5, 6\}$. Possible events include:
    - $A = \{2, 4, 6\}$: The event of rolling an even number.
    - $B = \{1, 3, 5\}$: The event of rolling an odd number.

### Operations on Events

Because the events are defined as subsets (therefore they are sets) we can apply [[Operations in sets]] in the events context.

- **Union**: The union of two events $A$ and $B$, denoted $A \cup B$, is the event that either $A$ or $B$ or both occur. $$A \cup B = \{x \in \Omega : x \in A \text{ or } x \in B\}$$
- **Intersection**: The intersection of two events $A$ and $B$, denoted$A \cap B$, is the event that both $A$ and $B$ occur.$$A \cap B = \{x \in S : x \in A \text{ and } x \in B\}$$
- **Complement**: The complement of an event $A$, denoted $A^c$, is the event that $A$ does not occur. $$A^c = \{x \in S : x \notin A\}$$