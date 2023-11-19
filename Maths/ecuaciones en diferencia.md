Las ecuaciones en diferencias son ecuaciones matemáticas que describen la relación entre los términos sucesivos de una secuencia o de [[sucesiones]]. Estas ecuaciones expresan cómo un término en la secuencia depende de uno o varios términos anteriores. En otras palabras, proporcionan una regla o fórmula que permite calcular un término de la secuencia en función de los términos previos.

Las ecuaciones en diferencias son especialmente útiles para modelar fenómenos que evolucionan en pasos discretos en lugar de forma continua. Son un concepto importante en diversas áreas de las matemáticas aplicadas, como la teoría de sistemas dinámicos, la teoría de control, la teoría de recursividad y la teoría de juegos, entre otras.

La forma implícita de escribir [[sucesiones]] es por medio de una ecuación en diferencia, por ejemplo:

$$X_{t+1} = X_t + 3$$

Las ecuaciones en diferencias pueden variar en complejidad, desde simples relaciones lineales hasta ecuaciones no lineales y sistemas de ecuaciones que involucran múltiples secuencias. Son herramientas esenciales en la modelización y el análisis de sistemas discretos en muchas disciplinas científicas y técnicas.

# Equilibrio en Ecuaciones en Diferencia

Un punto de equilibrio en una ecuación en diferencia se refiere a un valor o conjunto de valores para las variables involucradas en la ecuación, en los cuales la secuencia o sistema de ecuaciones no experimenta cambios con el paso del tiempo. En otras palabras, es un estado en el cual los términos futuros de la secuencia son idénticos a los términos actuales, indicando una estabilidad a lo largo del tiempo. formalmente se podría expresar como:

Sea $X_{t+1} = f_{(x_t)}$ una *EED*, decimos que $x^*$ es un punto de equilibrio o punto fijo de la *EED*, si se cumple que $x^* = f_{(x^*)}$, es decir, $X_{t+1} = X_t = x^*$
# Métodos de solución de Ecuaciones en Diferencia

## Método iterativo

El método tentativo o iterativo es una técnica utilizada para encontrar soluciones aproximadas de ecuaciones en diferencia, especialmente cuando no es posible obtener soluciones analíticas exactas de manera directa. Este método implica realizar sucesivas iteraciones, aplicando una regla o fórmula iterativa en cada paso para aproximar los valores de los términos de la secuencia.

En el contexto de una ecuación en diferencia, el método iterativo implica comenzar con un valor inicial y aplicar repetidamente la regla de la ecuación para calcular el siguiente término en función del valor anterior. Luego, este nuevo valor se convierte en el valor anterior para la siguiente iteración, y así sucesivamente. A medida que se realizan más iteraciones, se espera que los valores se acerquen a la solución deseada o converjan hacia un punto de equilibrio si existe.

## Método general

