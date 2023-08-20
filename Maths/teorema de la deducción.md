Sean $\alpha_1, ... , \alpha_n, \alpha, \beta$ proposiciones. 
$$\text{Si: } \alpha_1, ... , \alpha_n,\alpha \vDash \beta$$
$$\text{Entonces: } \alpha_1, ... , \alpha_n \vDash (\alpha \rightarrow \beta) $$
# Demostración

Por hipótesis $\alpha_1, ... ,\alpha_n, \alpha \vDash \beta$, es decir, por definición de [[implicación semántica]], $\alpha_1, ... , \alpha_n, \alpha \rightarrow \beta$ es una [[tautología]], queremos ver si $\alpha_1, ... , \alpha_n \rightarrow (\alpha \rightarrow \beta)$ por lo cual vamos a demostrar que:
$$
 (\alpha_1\wedge, ... ,\wedge \alpha_n) \rightarrow (\alpha \rightarrow \beta)
$$
es una [[tautología]]

para hacer esta demostración es fundamental recordar que la implicación solo es falsa cuando el antecedente es verdadero y el consecuente es falso, por ende vamos a suponer que $(\alpha \rightarrow \beta) = F$, esto implica que $\beta = F$ y $\alpha = V$, como sabemos por hipótesis que $(\alpha_1\wedge, ... ,\wedge \alpha_n \wedge \alpha) = F$  pero tenemos que $\alpha = V$, por tanto existe un $\alpha_i$ entre $(\alpha_1\wedge, ... ,\wedge \alpha_n)$ que es falso lo cual implica que: $(\alpha_1\wedge, ... ,\wedge \alpha_n) = F$, 

Se concluye entonces que si $\alpha_1, ... , \alpha_n,\alpha \vDash \beta$ Entonces $(\alpha_1 \wedge, ... \wedge \alpha_n) \rightarrow (\alpha \rightarrow \beta)$ es una [[tautología]] 