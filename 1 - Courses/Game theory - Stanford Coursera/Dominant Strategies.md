#GameTheory 

After define Dominant Strategies it's important to understand What is a Strategy, we can say a priori that a strategy is the set of action I define to do, We are calling this [[Pure Strategy]].

Let $s_i$ and $s'_i$ be two strategies for player $i$ and let $S_{-i}$ be the set of all possible strategy profiles for the other players.

Then we say $s_i$ **strictly dominates** $s'_i$ if  $\forall s_{-i} \in S_{-i}, u_i(s_i, s_{-i}) > u_i(s'_i, s_{-i})$   we can also say $s_i$ **very weakly dominates** $s'_i$ if  $\forall s_{-i} \in S_{-i}, u_i(s_i, s_{-i}) \geq u_i(s'_i, s_{-i})$

This means that a strategy $a$ strictly dominates another strategy $b$ if doesn't matter the choose my opponent do, still for me choose $a$ is better than $b$ when we extend this definition to "better or indifferent" we call it weakly dominates.

Dominant strategies are important because when I have one, I don't need to think about what the other players will do, if one strategy dominates all other, we say it is dominant. Also if an equilibrium are reached by strictly dominant strategies, this equilibrium must be unique. 

A strategy profile $(s_1^*, s_2^*, \dots, s_N^*)$  where each $s_i$ $\forall i$ are dominant strategies must be a [[Nash equilibrium]]

## Example

![[Pasted image 20241209103645.png]]
