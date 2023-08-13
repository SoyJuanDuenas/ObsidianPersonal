Una sucesión es una secuencia ordenada de puntos, otra forma de definirlas es como una función que va desde los números naturales hacia los reales.

$$
\mathbb N \rightarrow \mathbb R
$$
$$
t \rightarrow f_{(t)} = x_t
$$
Se puede pensar como una lista de números escritos en un orden definido, el historial de las sucesiones terminan generando [[time series models]].
# Representación de sucesiones

Existen 2 diferentes maneras de representar una sucesión
## Forma explicita

En la forma explicita detallamos todos los elementos de la secuencia

$$
\{x_1, x_2,x_3\} = \{X_t\}_{t=0}^{\infty} = \{1 + 3t\}_{t=0}^{\infty}
$$
## Forma implícita

Expresamos por medio de una ecuación que me describa la secuencia de la sucesión

$$
x_{t+1} = x_t + 3; x_0 = 1
$$

# Convergencia de una sucesión

diremos que una sucesión $\{X_t\}$ tiene un punto de convergencia L si su limite cuando t tiende a infinito existe, en caso contrario, la sucesión es divergente

$$
\lim_{t \rightarrow \infty} X_t = L
$$
 
## Teorema

Si $\lim_{t \rightarrow \infty} |X_t| = 0$ entonces la sucesión converge a cero

## Teorema del emparedado

Sean $X_t,Y_t,Z_t$ sucesiones, si $X_t \leq Y_t \leq Z_t$ para todo $t$, y  $\lim_{t \rightarrow \infty} X_t = L$ y  $\lim_{t \rightarrow \infty} Z_t = L$,  entonces  $\lim_{t \rightarrow \infty} Y_t = L$



	verificar el comportamiento de la sucesión de r^n