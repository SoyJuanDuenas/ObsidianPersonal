## Definition

The **Power Set** of a set $S$ is the set of all possible subsets of $S$, including the empty set and $S$ itself. If $S$ has $n$ elements, the Power Set of $S$ will have $2^n$ elements, this because [[Multiplication Rule]].
## Notation

The Power Set of a set $S$ is usually denoted as $\mathcal{P}(S)$ or $2^S$.

## Examples

### Example 1: Power Set of $\{a, b\}$

Let's consider the set $S = \{a, b\}$.

The Power Set of $S$ is: $\mathcal{P}(S) = \{\emptyset, \{a\}, \{b\}, \{a, b\}\}$

### Example 2: Power Set of \(\{1, 2, 3\}\)

For the set $S = \{1, 2, 3\}$:

The Power Set of \( S \) is:
$\mathcal{P}(S) = \{\emptyset, \{1\}, \{2\}, \{3\}, \{1, 2\}, \{1, 3\}, \{2, 3\}, \{1, 2, 3\}\}$

## Properties

1. **Cardinality**: If a set $S$ has $n$ elements, the Power Set of $S$ will have $2^n$ elements.
2. **Inclusion**: Every subset of $S$ is an element of the Power Set of $S$.
3. **Empty Set**: The Power Set always includes the empty set $\emptyset$.
4. **Set Itself**: The Power Set always includes the set $S$ itself.

## Construction

To construct the Power Set of a set \( S \):

1. Start with the empty set: $\emptyset$.
2. For each element in $S$ add it to all existing subsets to create new subsets.
3. Repeat until all elements of $S$ have been processed.
## Applications

Power Sets have applications in various fields including:

1. **Mathematics**: Used in combinatorics and probability.
2. **Computer Science**: Important in database theory, data mining, and the design of algorithms.
3. **Logic**: Used in the study of Boolean algebras and propositional logic.
4. **Set Theory**: Fundamental in the study of different infinities and the structure of sets.
