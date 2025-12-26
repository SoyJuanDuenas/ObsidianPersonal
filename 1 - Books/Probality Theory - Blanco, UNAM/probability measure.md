#probability 
# Definition

A **probability measure** is a function $P$ that assigns a real number to each event in a sample space $\Omega$ in a way that satisfies the [[probability axioms]]. It provides a formal way to quantify the likelihood of different outcomes in a [[random experiment]]
# Formal Definition

A probability measure $P$ on a [[sample space]] $\Omega$ with a [[sigma algebra]] $\mathcal{F}$ (a collection of subsets of $\Omega$) is a function $$P: \mathcal{F} \to [0, 1]$$ that satisfies

![[probability axioms]]

# Probability measure over $\mathbb{R}$

Let's be a [[random variable]] $X$ over a [[Probability space]] $(\Omega, \mathcal{F}, P)$, for each interval $(-\infty, x) \subseteq \mathbb{R}$ we can define the following [[random variable]]:

$$P_x((-\infty, x]) = P(X \in (-\infty, x])$$
The measure condition in the definition of a [[random variable]] guarantee that the set $X \in (- \infty, x] \in \mathcal{F}$ and for this reason can apply the [[probability measure]] $P$, with this in mind  $P_x$ can be extended to a [[probability measure]] over $\mathcal{B}(\mathbb{R})$ resulting in the following [[Probability space]] 

$$(\mathbb{R}, \mathcal{B}(\mathbb{R}), P_x)$$
