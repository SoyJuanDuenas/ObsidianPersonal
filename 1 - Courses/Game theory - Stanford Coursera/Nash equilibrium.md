#GameTheory 

A Nash Equilibrium is a fundamental concept in Game Theory where no player can gain a better payoff by unilaterally changing their strategy, assuming the other players keep their strategies unchanged. In essence, it represents a situation where all players are making the best decisions they can, given the decisions of others.

Under Nash Equilibrium nobody has an incentive to deviate from their action if an equilibrium profile is played.

In a strategic game with $N$ players:

- Let $A_i$​ denote the **strategy set** for player $i$, where $i \in \{1, 2, \dots, N\}$.
- Let $u_i(a_1, a_2, \dots, a_N)$ represent the **payoff function** for player $i$, which depends on the strategies chosen by all players.

A strategy profile $(a_1^*, a_2^*, \dots, a_N^*) \in A_1 \times A_2 \times \cdots \times A_N$ is a **Nash Equilibrium** if:
$$u_i(a_1^*, a_2^*, \dots, a_i^*, \dots, a_N^*) \geq u_i(a_1^*, a_2^*, \dots, a_i, \dots, a_N^*)$$
For every player $i$ and for all alternative strategies $a_i \in A_i$.