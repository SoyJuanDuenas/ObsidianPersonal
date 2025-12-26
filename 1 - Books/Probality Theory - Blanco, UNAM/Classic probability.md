#probability 

Let's be $E$ a [[random experiment]] with not infinity [[sample space]] $\Omega$. and all elements of $\Omega$ are equally likely to occur (Equiprobable [[sample space]]), Classic probability of a [[event]] is defined as follows:

$$P(A) = \frac{\#A}{\#\Omega}$$
In Spanish is the same than *"Casos posibles sobre casos favorables"*

To apply classic probability we need to know the number of elements (#) of some set, this could become in a expensive task, so it's important understand [[Counting Techniques]]

## Properties

1. $P(\Omega) = \frac{\#\Omega}{\#\Omega} = 1$
2. $P(A) = \frac{\#A}{\#\Omega} \geq 0$
3. If $A$ and $B$ are [[disjoint sets]] then $P(A \cup B) = \frac{\# (A \cup B)}{\#\Omega} = \frac{\#A + \# B}{\#\Omega} = P(A) + P(B)$
4. Generalizing, if $A_1, A_2, \dots$ are [[disjoint sets]] then we have $$P(\bigcup_{i=1}^{\infty} A_i) = \sum_{i=1}^{\infty} P(A_i)$$
