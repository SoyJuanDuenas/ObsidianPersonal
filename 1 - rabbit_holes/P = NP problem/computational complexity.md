#ComputerScience 

**Computational Complexity** is a branch of theoretical computer science that studies the resources required (such as time and space) to solve computational problems. It classifies problems based on the inherent difficulty of solving them and the efficiency of algorithms that provide solutions.

---
### Key Concepts

1. **Resources**:
    - **Time Complexity**: The amount of time an [[algorithm]] takes to complete, typically expressed as a function of the input size $n$.
    - **Space Complexity**: The amount of memory an algorithm uses during execution.
2. **Asymptotic Analysis**:
    - Uses **[[Big-O Notation]]** to describe the upper bound of an algorithm’s growth rate, helping to compare efficiencies of algorithms.
3. **Decision Problems**: Questions with yes/no answers form the basis for most complexity classes.
4. **Reductions**: Transforming one problem into another to show relationships between their complexities.
---
### Complexity Classes

#### Common Complexity Classes:

1. **[[P - Problems]] (Polynomial Time)**: Problems solvable in polynomial time by a deterministic Turing machine.
2. **[[NP - Problems]] (Nondeterministic Polynomial Time)**: Problems for which proposed solutions can be verified in polynomial time.
3. **[[NP - Complete Problems]]**: The hardest problems in NP. Solving one in polynomial time would imply [[P = NP]].
4. **NP-Hard**: Problems at least as hard as the hardest problems in NP but not necessarily in NP.
5. **PSPACE**: Problems solvable using polynomial space, regardless of time.
6. **EXPTIME**: Problems solvable in exponential time.
---
### Types of Problems

1. **Tractable Problems**: Problems in $P$, solvable efficiently in practice.
2. **Intractable Problems**: Problems requiring exponential or higher time/space, such as those in NP-Hard.
3. **Undecidable Problems**: Problems for which no algorithm can determine an answer (e.g., the Halting Problem).
---
### Tools for Analysis

1. **[[Turing Machine]]**: Theoretical models for defining and analyzing complexity.
2. **[[Big-O Notation]], [[Omega Notation]], and [[Theta Notation]]**: Describe the upper, lower, and tight bounds of algorithms.
3. **[[Reductions]]**: Prove the hardness of problems by transforming them into known difficult problems.

