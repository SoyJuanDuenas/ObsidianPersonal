Para este escrito nos basaremos en:

>**Increasing Risk: A Definition And It's Economic Consequences
> Rothschild and Stiglitz (1969)**

Este paper trata de responder dos preguntas

- ¿ Cuándo es una variable aleatoria y cuando es más variable que otra variable aleatoria X ?
- ¿ Que efectos tiene un aumento en la variabilidad de la incertidumbre en el comportamiento económico y si este aumento en el riesgo de oportunidad de inversión lleva a más o menos ahorros ?

Antes de llevar a cabo este resumen es mejor antes recordar que nos trae a este paper y por ende cual es el objeto de estudiar este paper y es la influencia que ejerció sobre [[Atkinson (1970)]], para esto es importante recordar en que puntos Atkinson lo mencionó o en que sentido lo mencionó.

1. Lo cita en un pie de pagina para resaltar que el interés en la pregunta de la medición de la desigualdad fue originalmente estimulada por la lectura de este paper.
2. Lo cita en un segundo pie de pagina haciendo referencia a que debido a que el campo de la toma de decisiones bajo incertidumbre ha tenido más atención que la medición de la desigualdad, va a tomar resultados de este campo, entre los cuales esta señalado este paper.
3. El principio de la transferencias de [[Dalton (1920)]] es el mismo concepto de "Mean preserving spread" introducido por este paper. Además, [[Atkinson (1970)]] compara ambos conceptos en figuras simultaneas.
4. De nuevo recuerda el termino de "Mean preserving spread" para demostrar de que en transferencias infinitesimales no necesariamente son proporcionales.

Es por esto que nos concentraremos en el termino de "Mean Preserving Spread" sin necesidad de entrar en detalles del campo de toma de decisiones bajo incertidumbre. Únicamente detallaremos lo necesario para entender el concepto a profundidad.

# ¿ Cuándo es una variable aleatoria y cuando es más variable que otra variable aleatoria X ?

Rothschild and Stiglitz inician respondiendo la primera pregunta planteada diciendo que hay al menos 5 aproximaciones distintas para responder:

## 1. $Y$ es igual a $X$ más ruido

Si simplemente añadimos un ruido independiente a una variable aleatoria diremos que la nueva variable aleatoria es más riesgosa (variable o tal vez con mayor varianza) que la variable aleatoria original, supongamos que:

$$
Y = X + Z
$$
donde $>$ es una variable aleatoria que es independiente respecto a $X$, tal que:
$$
E(Z|X) = o
$$
$$
\text{Para toda X}
$$

note que $Y$ y $X$ tienen la misma media

## 2. Todo individuo con aversión al riesgo prefiere $X$ a $y$

En la teoría de la maximización de la utilidad, un individuo con aversión al riesgo es tal que tiene una función de utilidad cóncava y si $X$ y $Y$ tienen la misma media va a preferir la de menor riesgo.

$$
E(U(X)) > E((Y)) 
$$

Por lo cual es razonable decir que $X$ es menos riesgoso que $Y$

## 3. $Y$ tiene más peso en las colas que $X$

Si $X$ y $Y$ tienen funciones de densidad $F$ y $G$ respectivamente y $G$ fue obtenida de $F$ manteniendo la misma media pero añadiendo valores en las colas, es razonable decir que $Y$ es más incierta que $X$

## 4. $X$ es una mezcla de $Y$

Supongamos que $Y$ es una variable aleatoria con media $\mu$ y sea $Y'$ una variable aleatoria que es igual a $\mu$ con probabilidad de 1. Por lo tanto si $X$ hace parte de la combinación lineal entre $Y$ y $Y'$ entonces $X$ es menos riesgoso que $Y$.

## 5. $Y$ tiene una varianza mayor a la de $X$

normalmente las comparaciones de riesgo o incertidumbre son normalmente restringidas a comparaciones de la varianza, esto atribuido a la larga historia del uso de la varianza como medida de dispersión en la teoría estadística.

El principal aporte de el paper de Rothschild and Stiglitz es que las cuatro primeras aproximaciones llevan a una sola definición de mayor riesgo, diferente a la quinta aproximación, además se demuestra que no se puede igualar el riesgo de $X$ con la varianza de $X$ lo cual sugiere que el concepto de Rothschild y Stiglitz de aumento de riesgo es mejor que el estándar relacionado con la varianza.

# Mean preserving spread

El concepto de "mean-preserving spread" (distribución que conserva la media) fue introducido por Rothschild and Stiglitz(1969). Este concepto se utiliza para comparar y analizar cambios en distribuciones de probabilidad, especialmente en el contexto de riesgo e incertidumbre.

En el contexto de la "mean-preserving spread", hay dos ideas principales:

1. **Conservación de la Media**: Esta parte del concepto se refiere a la idea de que un cambio en la distribución de probabilidad conserva la media (o valor esperado) si la media de la distribución permanece inalterada después del cambio. En otras palabras, si calculas el promedio de los resultados antes y después del cambio, será el mismo. Esto significa que, en promedio, no hay cambio en la "tendencia central" de la distribución.

2. **Spread o Dispersión**: El término "spread" se refiere a la dispersión o variabilidad de los resultados en una distribución de probabilidad. Si imaginas una distribución como un gráfico, el spread se refiere a cuán "extendidos" están los puntos de datos alrededor de la media. Es una medida de la incertidumbre o el riesgo asociado con la distribución.

Al combinar estas dos ideas, una "mean-preserving spread" se puede entender como un cambio en la distribución de probabilidad de los resultados de manera que no altera el resultado promedio (media), pero podría afectar el grado de incertidumbre o variabilidad (spread) alrededor de esa media. En otras palabras, el rango de resultados se vuelve más amplio o estrecho manteniendo constante el resultado promedio.

Ahora es importante revisar el concepto de transferencias de [[Dalton (1920)]] para comparar matemática y teóricamente ambos conceptos que [[Atkinson (1970)]] luego retoma.