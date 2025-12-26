#GameTheory 

Best response is a consequence of [[Nash equilibrium]], if I know what everyone else was going to do, It would be easy to pick our own action.

Let's say $a_{-i}$ are the action sequence of everybody except us, player $i$

$$a_i = \{a_1, \dots , a_{i-1},a_{i+1}, \dots, a_n\}$$
this means that we can reformulate $a$:
$$a = (a_{-i}, a_i)$$
With this in mind we can make a definition, the best response are defined as:

$$a_i^* \in BR(a_{-i}) \text{ iff for all } a_i \in A_i, u_i(a_i^*, a_{-i}) \geq u_i(a_i, a_{-i})$$
Then the best response are the choose that I can take and are at least as great as anything else I might choose.

From this perspective I can also make a alternative definition of [[Nash equilibrium]]

$$a = (a_1, \dots, a_n) \text{ is a pure strategy nash equilibrium iff } \forall i, a_i \in BR(a_{-i})$$
this mean that a profile are Nash Equilibrium if all players accomplish their best response.