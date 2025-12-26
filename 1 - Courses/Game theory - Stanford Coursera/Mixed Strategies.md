#GameTheory 

In some types of games we would want to play in a stochastic form, not a deterministic (like in [[Pure Strategy]]) the idea behind the mixed strategies are confuse the opponent by playing randomly.

Let's define a strategy $s_i$ for agent $i$ as any probability distribution over the actions of $A_i$, then when we talk abaut mixed strategy more than one action is played with positive probability. A useful example is say instead I will play Coss ,I will play the output of this flip coin.

If the players follow mixed strategy profiles we cannot get the payoff because we will not always end in the same cell. To solve this situation we wil use the concept of [[expected utility]] from decision theory. Where:

$$u_i(s) = \sum_{a\in A} u_i(a)Pr(a|s)$$
$$Pr(a|s) = \prod_{j \in N}s_j(a_j)$$
The utility under mixed strategy is equal to the sum of all action of the game where we take the utility of each cell and multipy for the probability of the realization of this cell.

Mixed strategy could be interpreted in different ways, mixed strategies are a concise description of what might happen in repeated play for example if we count pure strategies in the limit. Mixed strategiesa can be described also as population dynamics, 2 agents chosen fron a population, all having deterministic strategies. mixed strategies gives the probability of getting each [[Pure Strategy]]. 
