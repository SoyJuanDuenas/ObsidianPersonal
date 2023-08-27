La estimación puntual de un parámetro en el contexto de la [[inferencia estadística]] se refiere al proceso de calcular un único valor numérico que se utiliza como una mejor conjetura o estimación del valor real de un parámetro poblacional desconocido. En otras palabras, es un intento de adivinar cuál es el valor de un parámetro de interés basado en la información proporcionada por una muestra de datos.

para estimar un parámetro $\theta$ es necesario obtener una muestra aleatoria y a partir de esta muestra aleatoria, calcular un *estimador puntual / parámetro puntual* $\hat{\theta}$ el cual es una función de la muestra aleatoria, existen infinitos estimadores de $\theta$. Parte fundamental de la estadística es usar herramientas para compararlos y escogerlos.

# Propiedades de los estimadores

- $\hat{\theta}$ es una variable aleatoria
- $\hat{\theta}$ depende de la muestra usada
- $\hat{\theta}$ tiene una [[función de distribución|función de distribución]]
# Evaluación de estimadores

Podemos hablar de otras propiedades de los estimadores por medio del cual podemos evaluarlo.
## Sesgo

Un estimador es insesgado si en promedio es el parámetro poblacional, por lo cual podemos decir que el sesgo se calcula como:

$$
sesgo(\theta) = E(\hat{\theta}) - \theta
$$
## Eficiencia

la eficiencia puede ser definida como que tanto nos demoramos en llegar con el estimador muestral al parámetro poblacional, esta puede ser definida como la varianza del parámetro muestral.

$$
var(\hat{\theta})
$$
## Consistencia

la consistencia es que a mayor muestra la probabilidad de que el estimador sea igual al poblacional es casi o converge a 1

$$
\lim_{n \rightarrow \infty} P(\hat{\theta}) = \theta
$$
