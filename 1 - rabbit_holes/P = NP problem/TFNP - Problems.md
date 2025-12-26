#ComputerScience 

In [[computational complexity]] theory, the complexity class TFNP is the class of total function problems which can be solved in nondeterministic polynomial time. That is, it is **the class of function problems that are guaranteed to have an answer**, and this answer can be **checked** in polynomial time, or equivalently it is the subset of [[FNP - Problems]] where a solution is guaranteed to exist. The abbreviation TFNP stands for "Total Function Nondeterministic Polynomial".

The class TFNP is formally defined as follows.

A binary relation $P(x,y)$ is in TFNP if and only if there is a deterministic polynomial time algorithm that can determine whether $P(x,y)$ holds given both $x$ and $y$, and for every $x$, there exists a $y$ which is at most polynomially longer than $x$ such that $P(x,y)$ holds.