Definimos la implicación semántica como: 

Sean $\alpha_1,\alpha_2,\alpha_3, ..., \alpha_n, \beta$ proposiciones, diremos que $\alpha_1, ... , \alpha_n$ implica semánticamente a $\beta$ , si y solo si:
$$(\alpha_1 \wedge \alpha_2 \wedge , ... , \wedge \alpha_n) \rightarrow \beta$$
es una [[tautología]]. 

Denotamos la implicación semántica como:
$$
\alpha_1, ... , \alpha_n \vDash \beta
$$
# Observación

Recordemos que la implicación solo es falsa cuando el antecedente es verdad y el consecuente es falso, por lo tanto si $\beta = F$, obliga a $(\alpha_1 \wedge \alpha_2 \wedge , ... , \wedge \alpha_n) = F$, recordando las tablas de verdad de la conjunción, para algún $i, \alpha_i =F$, ie, al menos una de las alphas debe ser falsa.

# Ejemplo

Sean $\alpha$ y $\beta$ proposiciones dadas

$$
\alpha \rightarrow \beta, \alpha \vDash \beta
$$
Este ejemplo es denominado [[Modus Ponens]] 
## Solución: 

$$
\text{debemos ver que: } ((\alpha \rightarrow \beta)\wedge \alpha) \rightarrow \beta
$$
es una [[tautología]]
### Argumentación

Supongamos que el consecuente $\beta = F$, si $\alpha = F$ entonces el antecedente $((\alpha \rightarrow \beta)\wedge \alpha)) = F$ y no habría problema. sin embargo si $\alpha = V$, pero supusimos que $\beta = F$ entonces $(\alpha \rightarrow \beta) = F$ y por lo tanto el antecedente $((\alpha \rightarrow \beta)\wedge \alpha)) = F$.

Luego, $((\alpha \rightarrow \beta)\wedge \alpha) \rightarrow \beta$ es una [[tautología]]

# Ejemplo

sean $\alpha$ y $\beta$ proposiciones dadas
$$
\alpha \wedge \beta \vDash \alpha 
$$
## Solución

Debemos verificar si se cumple y bajo que condiciones se cumple que:

$$
\alpha \wedge \beta \rightarrow \alpha
$$
es [[tautología]]

## Argumentación: 

Dado que la única manera en la cual la implicación es falsa es que el antecedente sea verdadero y el consecuente sea falso, suponemos $\alpha = F$. Por lo cual siempre el antecedente $\alpha \wedge \beta$ será falso y por lo tanto la implicación $\alpha \wedge \beta \rightarrow \alpha$ será una tautología.


