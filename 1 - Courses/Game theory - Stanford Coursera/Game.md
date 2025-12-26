#GameTheory

A Game in Game Theory is any interaction between two or more people, where the outcomes of the interaction depend on everybody does and everybody has different levels of happiness for the different outcomes and also all players are [[Self interested agents]]

We can desegregate the components of a game in the following categories:

- **Players:** The entity who makes the decision.
- **Actions:**  Are the possible decisions that the players can make.
- **Payoffs** This are the motivations of the player, benefit of choose a particular action or another action. 

When we're talking about this framework there is a particular questions that we can make us:

- What actions should a player of the game take ? 
- Would all users behave the same in this scenario ?
- What global behavior patterns should a system designer expect ?
- For what changes to the numbers would behavior be the same ?
- What effect would communication have ?
- Is there any repetitions ? the repetitions are finite or infinite ?
- Foes it matter if I believe that my opponent is rational ? 

This questions are going to show us relevant concepts or guide us to a specifical type of games.

# Representation of a game

There are two standard representation of a game

1. **Normal form / matrix form / Strategic form**: It list what payoffs get as a function of their actions. It's perfect when the players make the decision simultaneously but strategies encode many things.
2. **Extensive form** This form includes timing of moves, here the players move sequentially and it is represented as a tree, let us keep track of what each player know when he or she makes each decision.

## Normal form

A finite, n-person normal form game follows $\langle N, A, u \rangle$.

- **Players:** $N = \{1,\dots , n\}$ is a finite set of $n$, indexed by $i$
- **Action set** are going to be for each player, then action set for player $i$ are $A_i$ Here we cand file also **profile actions** that are a list for what are another players doing $a = (a_1, \dots, a_n) \in A = A_1 \times \dots \times A_n$
- **[[utility function]] or payoff function:** for player $i:$ $u_i: A \rightarrow \mathbb{R}$ a function of all the actions that are played What's the payoff for the different players. here we can find also profile utility functions $u = (u_1, \dots , u_n)$

We can write a 2-player game as a matrix where row player are player 1 and column player are player 2, Rows correspond to actions $a_1 \in A_1$, columns correspond to actions $a_2 \in A_2$ and cells list the utility values for each player (row, column)


![[Pasted image 20241204222437.png]]


If we desegregate this example into the parts we're going to see the following situation

- **Players:**  There is two players in this game. 
$$N = \{P1,P2\}$$
- **Action set**  Each player can choose Cooperate or Defeat 
$$A_1 = \{C,D\}; A_2 = \{C,D\}$$
- **Total possible profile actions:** Each profile action are the combination of the player's actions sets, then to have all possible combinations we should apply [[Cartesian product]] to each action set, in this example 
$$A = A_1 \times A_2 = \{(C,C),(C,D),(D,C),(D,D)\}$$
Now to understand the profile actions and how the [[utility function]] are used in game theory let's denote the profile actions as:
$$a = (a_1, a_2)$$
Where $a_1 \in A_1$ are the action choose by player 1 and $a_2 \in A_2$ are the action choose by player 2.

If we suppose that player 1 choose C and player 2 choose D, then the profile action are going to be:
$$a = (C,D)$$
Now, with the profile action and the [[utility function]] expressed as a matrix in the game, we can say that:
$$u_1(a) = -4; u_2(a) = 0$$




