The Support Enumeration Method is a systematic approach to compute [[Nash equilibrium]] in finite games by identifying all possible combinations of active strategies ([[Support]]) for the players. This method is particularly useful for games with small strategy spaces, as it explicitly considers all feasible strategy supports.

 if we fix the [[support]] of the strategies of the player, then the problem becomes very easy, and we can set it up as a linear program and solve it efficiently. 

Indeed, there are an exponential number  of supports to explore. And so the trick in this procedure is to explore them cleverly using clever [[heuristics]]. 

although, the ladder procedure is not as smart or as insightful as the  [[Linear Complementarity Problem formulation]] aproach, it turns out that in practice tends it tends to run very fast.

