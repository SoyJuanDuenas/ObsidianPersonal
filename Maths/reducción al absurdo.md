La reducción al absurdo hace parte de las  [[técnicas de demostración]] y nos sirve para probar teoremas, este método usa la [[implicación semántica]] y parte de la siguiente proposición:

Sean $\alpha_1, ... , \alpha_n, \beta$ proposiciones, y sea $\perp$ una [[contradicción]]

$$
\text{si: } \alpha_1, ... , \alpha_n, \neg \beta \vDash \perp
$$
$$
\text{Entonces: } \alpha_1, ... , \alpha_n \vDash \beta
$$
O dicho de otra manera, "Suponer que a lo que se quiere llegar como hipótesis negativa y llegar a una contradicción"

# Demostración

Tenemos que por hipótesis, que $\text{si: } (\alpha_1 \wedge ... \wedge \alpha_n \wedge \neg \beta) \rightarrow \perp$ es una [[tautología]], por lo tanto siempre $(\alpha_1 \wedge ... \wedge \alpha_n \wedge \neg \beta) = F$, queremos demostrar que $(\alpha_1\wedge ... \wedge \alpha_n) \rightarrow \beta$ es una [[tautología]]

Dado que la única manera en la cual la implicación es falsa es que el antecedente sea verdadero y el consecuente sea falso, suponemos que $\beta = F$ por lo tanto, $\neg \beta = V$, pero tenemos que por hipótesis que $(\alpha_1 \wedge ... \wedge \alpha_n \wedge \neg \beta) = F$ lo cual se sigue que existe algún $j = 1, ...,n$ tal que $\alpha_j = F$.

Por lo tanto concluiremos que $(\alpha_1\wedge ... \wedge \alpha_n) \rightarrow \beta$ es una [[tautología]] 