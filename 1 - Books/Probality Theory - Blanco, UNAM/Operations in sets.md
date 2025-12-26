Operations in set theory are the fundamental processes by which new sets are constructed from existing sets. These operations include union, intersection, difference, complement, symmetric difference, power set and Cartesian product. Each operation has specific rules that determine how elements from the involved sets are combined or manipulated to form a new set. These operations are essential for understanding relationships between sets and for performing various mathematical and logical tasks within the framework of set theory.

A important theorem to simplify operations in sets are [[Morgan Laws]]

## Union (∪):

The union of two sets A and B is the set containing all elements that are in A, in B, or in both. Mathematically, 

$$A \cup B = \{ x \mid x \in A \text{ or } x∈B\}$$
![[Pasted image 20240613190504.png ]]

Applying this operation to a A and B [[event]]s and [[sample space]] we can obtain some properties:

- $A \cup B = B \cup A$
- $A \cup A = A$
- $A \cup \emptyset = A$
- $A \cup \Omega = \Omega$
- $A \cup A^{c} = \Omega$

The associative and distributive law apply to this operation, therefore:

- $A \cup (B \cup C) = (A \cup B) \cup C = A\cup B \cup C$
- $A \cup (B \cap C) = (A \cup B) \cap (A \cup B)$

This operation can be done for more than a pair of sets, with the following notation we can generalize this operation:

$$A_1 \cup A_2 \cup A_3 \cup \dots \cup A_n = \bigcup_{i=1}^{n} A_i$$
Then this symbol means "some of the $A_i$ [[event]]s happens" and also we can apply distributive and [[Morgan Laws]] to it

- $A \cap (\bigcup_{i=1}^{\infty}B_i) = \bigcup_{i=1}^{\infty}(A \cap B_i)$
- $(\bigcup_{i=1}^{n} B_i)^c = \bigcap_{i=1}^{n} B_k^c$
 

## Intersection (∩):

The intersection of two sets A and B is the set containing all elements that are both in A and in B. Mathematically, 
$$A \cap B = \{ w \in \Omega \mid w \in A \text{ and } w \in B \}$$
![[Pasted image 20240613192609.png]]
Applying this operation to a A and B [[event]]s and [[sample space]] we can obtain some properties:

-  $A \cap B = B \cap A$
- $A \cap A = A$
- $A \cap \emptyset = \emptyset$
- $A \cap \Omega = A$
- $A \cup A^{c} = \emptyset$

The associative and distributive law apply to this operation, therefore:

- $A \cap (B \cap C) = (A \cap B) \cap C = A\cap B \cap C$
- $A \cap (B \cup C) = (A \cap B) \cup (A \cap B)$

This operation can be done for more than a pair of sets, with the following notation we can generalize this operation:

$$A_1 \cap A_2 \cap A_3 \cap \dots \cap A_n = \bigcap_{i=1}^{n} A_i$$
Then this symbol means "some of the $A_i$ [[event]]s happens" and also we can apply distributive and [[Morgan Laws]] to it

- $A \cup (\bigcap_{i=1}^{\infty}B_i) = \bigcap_{i=1}^{\infty}(A \cup B_i)$
- $(\bigcap_{i=1}^{n} B_i)^c = \bigcup_{i=1}^{n} B_k^c$

## Difference (−):

The difference of two sets A and B (also called the relative complement) is the set containing all elements that are in A but not in B. Mathematically, 
$$A - B = \{ w \in \Omega \mid x \in A \text{ and } x \not\in B \}$$
![[Pasted image 20240613193647.png]]
Applying this operation to a A and B [[event]]s and [[sample space]] we can obtain some properties:

-  $A - B \not = B - A$
- $A - A =  \emptyset$
- $A - \emptyset = A$
- $A - \Omega = \emptyset$
- $A - B = A - (A \cap B)$

## Complement ( $^{c}$ ):

The complement of a set A, relative to a universal set U, is the set of all elements in U that are not in A. Mathematically,
$$A^{c} = \{ x \in U \mid x \in U \text{ and } x \notin A \}$$
![[Pasted image 20240613204000.png]]
Applying this operation to a A and B [[event]]s and [[sample space]] we can obtain some properties:

-  $\emptyset^{c} = \Omega$
-  $\Omega^{c} = \emptyset$
-  $(A^{c})^{c} = A$
## Symmetric Difference (△):

The symmetric difference of two sets $A$ and $B$ is the set containing elements that are in either $A$ or $B$ but not in both. Mathematically, $$A \Delta B = (A - B) \cup (B - A)$$
![[Power set]]


![[Cartesian product]]


