#probability

## Notation:

Is important to make the difference between $X$ that is a function and $x$ that is a real number. 

# Definition

Let's be a [[Probability space]] $(\Omega, \mathcal{F}, P)$, a random variable $X$ is a function than:

$$X: \Omega \rightarrow \mathbb{R}$$

This definition should satisfy than for each $x \in \mathbb{R}$ (medibility condition)

$$\{w\in \Omega: X(w) \leq x\} \in \mathcal{F}$$

To illustrate this condition let see the following figure:


![[Pasted image 20240818141330.png]]


The medibility condition It's important because It let us to apply a [[probability measure]] $P$ over $\mathbb{R}$.

# Example

The random experiment will be flip a fair coin, the sample space will be head or tail, the sigma algebra is the power set of $2^\Omega$ and the probability measure will be $P( \text{ "head" } ) = P( \text{ "tail" } ) = \frac{1}{2}$ and the random variable will be:

$$X(\text{ "head" }) = 0$$$$X(\text{ "Tail" }) = 1$$
Then:

$P(X = 0) = P(x\in \{0\}) = \frac{1}{2}$
$P(X = 1) = P(x\in \{1\}) = \frac{1}{2}$
$P(X = 2) = P(x\in \{2\}) = 0$
$P(X \leq 0) =  \frac{1}{2}$
$P(X \geq 1) =  \frac{1}{2}$
$P(X \in (0,1)) = 0$
$P(X \in [0,1]) = 1$

# Discrete random variable

A random variable are a discrete random variable if can take a finite values or a countable set of values, typically:

$$\{0,1,2,\dots, n, \dots\} $$
# Continuos random variable

A random variable are continuous if can take all values of a $\mathbb{R}$ interval, typically:

$$(0,1)$$
$$(0,\infty)$$
$$(-\infty,\infty)$$


