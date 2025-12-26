#GameTheory 

Perfect Information Extensive Form Games are a type of [[game]] in game theory where all players have complete knowledge of the game's history at every decision point. This means that at any point in the game, each player knows all the previous moves made by all players, including themselves.

Now when we incorporate the **extensive form** of a game, we have a detailed representation that captures the sequential nature of decisions, the information available to players at each decision point, and the payoffs associated with different outcomes. This make the temporal structure explicit.

# Definition

A finite perfect information game in extensive form is defined by the tuple $(N, A, H, Z, \chi, \rho, \sigma, \mu)$

where:

- $N$ = **players**
- $A$ = **Actions**
- Choice nodes and labels for these nodes
	- $H$ = **Choice nodes**
	- $\chi : H \rightarrow 2^A$ = **Action Function**, Assigns to each choice node a set of possible actions
	- $\rho: H \rightarrow N$ = **player function**, Assigns to each non-terminal node $h$ a player $i \in N$ who chooses an action at $h$
- $Z$ = **Terminal nodes**: $Z$ is a set of terminal nodes, disjoint from $H$
- $\sigma: H \times A \rightarrow H \cup Z$ = **Successor function**, with this function we can create the edges of the [[tree]], $\sigma$ maps a choice node and an action to a new choice node or terminal node such that for all $h_1, h_2 \in H$ and $a_1, a_2 \in A$, if $\sigma (h_1, a_1) = \sigma (h_2, a_2)$ then $h_1 = h_2$ and $a_1 = a_2$ 
- $\mu = (\mu_1, \dots, \mu_n): u_i: Z \rightarrow \mathbb{R}$ **Utility Function** for player $i$ on the terminal nodes $Z$

# Pure strategies in a perfect information extensive form game

A Pure strategy for a player in a perfect information game is a complete specification of which action to take at each node belonging to each player, this could be thinking as giving instructions to another person to play the game for you. 

let $G = (N, A, H, Z, \chi, \rho, \sigma, \mu)$ be a perfect-information extensive form game. Then the [[Pure Strategy]] of player $i$ consist of the cross product:

$$\prod_{h \in H, \rho(h) = i} \chi (h)$$
# example

