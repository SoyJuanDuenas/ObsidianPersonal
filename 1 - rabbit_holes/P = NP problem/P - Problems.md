#ComputerScience 

In [[computational complexity]] theory, **P** (short for "Polynomial time") is the class of decision problems that can be solved by a deterministic [[Turing machine]] in polynomial time. This means that the time required to solve these problems grows at most polynomially with the size of the input.

### Key Characteristics

1. **Deterministic**: Problems in P can be solved using deterministic algorithms.
2. **Polynomial Time**: The runtime of the solving [[algorithm]] is expressed as $O(n^k)$, where $n$ is the input size, and $k$ is a constant.
3. **Feasibility**: Problems in P are often considered "efficiently solvable" in practice, though efficiency depends on the value of $k$ and constants in the polynomial.

---

### Formal Definition

Let $L$ be a language (or decision problem). $L \in P$ if there exists a deterministic [[Turing machine]] $M$ such that:

1. $M$ decides $L$: It halts and outputs "yes" or "no" for every input.
2. $M$'s runtime is bounded by a polynomial function of the input size $n$.

---
### Examples of Problems in P

1. **Sorting Algorithms**: Problems like sorting a list (e.g., QuickSort, MergeSort) are in P with runtimes like $O(n \log n)$.
2. **Graph Problems**:
    - Determining if a graph is connected.
    - Finding the shortest path in a graph (e.g., [[Dijkstra's algorithm]]).
3. **Arithmetic Operations**:
    - Addition, subtraction, multiplication, and division of integers.
4. **String Matching**: Finding substrings using algorithms like the Knuth-Morris-Pratt (KMP) [[algorithm]].

### Relation to Other Complexity Classes

- **P - problem vs. NP - problem**:  
    P - problems is a subset of [[NP - problems]] (Nondeterministic Polynomial time). If a problem is in P, it is also in NP because deterministic algorithms are a subset of nondeterministic ones.  
    The question of whether $P=NP$ is one of the most important unsolved problems in computer science.
    
- **P vs. NP-Complete**:  
    Problems in NP-Complete are both in NP and as hard as the hardest problems in NP. If any [[NP - problems]] can be solved in polynomial time, then [[P = NP]].
    
- **P vs. PSPACE**:  
    P is a subset of PSPACE (problems solvable in polynomial space). However, PSPACE includes problems that may not be solvable in polynomial time.