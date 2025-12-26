#ComputerScience 

In [[computational complexity]] theory, the complexity class FNP is the function problem extension of the decision problem class [[NP - Problems]]. The name is somewhat of a misnomer, since technically it is a class of binary relations, not functions, as the following formal definition explains:

A binary relation $P(x,y)$, where $y$ is at most polynomially longer than $x$, is in FNP if and only if there is a deterministic polynomial time [[algorithm]] that can determine whether $P(x,y)$ holds given both $x$ and $y$.

Where a single output (of a total function) is expected for every input, but the output is more complex than that of a decision problem. For function problems, the output is not simply 'yes' or 'no'.