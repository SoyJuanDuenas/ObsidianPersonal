#ComputerScience 

In [[computational complexity]] theory, **NP** (short for "Nondeterministic Polynomial time") is the class of decision problems for which a proposed solution can be **verified** in polynomial time by a deterministic [[Turing machine]]. This does not necessarily mean the problem can be solved in polynomial time—only that if a solution is provided, it can be quickly checked.

---
### Key Characteristics

1. **Verification, Not Solution**:  
    A problem is in NP if a candidate solution can be verified in polynomial time, even if finding that solution may take longer.
    
2. **Nondeterminism**:  
    Problems in NP can conceptually be solved in polynomial time by a nondeterministic [[Turing machine]], which can "guess" the correct solution from many possibilities.
    
3. **Polynomial Verification**:  
    If a solution exists, a deterministic machine can confirm it in $O(n^k)$ time, where $n$ is the size of the input, and $k$ is a constant.

---
### Formal Definition

Let $L$ be a language (or decision problem). $L \in NP$ if there exists a deterministic [[Turing machine]] $M$ and a polynomial $p(n)$ such that:

1. $M$ takes two inputs: the problem instance $x$ and a "certificate" $y$.
2. $M(x, y)$ runs in time $O(p(n))$ and outputs "yes" if $y$ is a valid certificate for $x$.

---
### Examples of NP Problems

1. **Boolean Satisfiability Problem (SAT)**: Determine if there exists an assignment of variables such that a given Boolean formula evaluates to true.
3. **Graph Coloring**: Can a graph's vertices be colored using $k$ colors such that no two adjacent vertices have the same color?
4. **Subset Sum Problem**: Given a set of integers, is there a non-empty subset whose sum equals a given number $k$?
5. **[[Hamiltonian Path]] Problem**: Does a path exist in a [[graph]] that visits each vertex exactly once?

---
### Relation to Other Complexity Classes

**NP-Complete Problems**:

- [[NP-Complete Problems]] are the "hardest" problems in NP.
- If any NP-Complete problem can be solved in polynomial time, then all NP problems can be solved in polynomial time ([[P = NP]]).


