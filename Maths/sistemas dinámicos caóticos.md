Un sistema dinámico caótico, también conocido simplemente como sistema caótico, es un tipo de sistema dinámico en el cual las pequeñas variaciones en las condiciones iniciales pueden conducir a resultados drásticamente diferentes en el futuro. Estos sistemas son altamente sensibles a las condiciones iniciales y muestran un comportamiento aparentemente impredecible o caótico a lo largo del tiempo, a pesar de que están gobernados por ecuaciones matemáticas deterministas.

 Para que un sistema dinámico sea un sistemas dinámicos caóticos se deben presentar las siguientes condiciones:

1. [[alta sensibilidad a las condiciones iniciales]]: Pequeñas diferencias en las condiciones iniciales conducen a trayectorias divergentes en el espacio de fase. Esto se conoce como el "efecto mariposa", donde el aleteo de una mariposa en un lugar del mundo podría, teóricamente, desencadenar un tornado en otro lugar.
2. Para predecir el futuro en un sistema caótico, el estado actual necesita conocerse con predicción infinita.
3. La separación entre dos soluciones del sistema dinámico con condiciones iniciales muy parecidas es de orden exponencial.

En los sistemas dinámicos caóticos podemos encontrar las siguientes características 

5. [[bifurcaciones]]: Los sistemas caóticos a menudo exhiben [[bifurcaciones]], que son puntos en los cuales el sistema cambia de un comportamiento estable a uno caótico o viceversa a medida que se ajustan ciertos parámetros.

6. Atractores extraños: En lugar de converger hacia un único punto o ciclo, los sistemas caóticos a menudo exhiben comportamientos en forma de atractores extraños en el espacio de fase, que son conjuntos no periódicos pero limitados. Estos atractores tienen una estructura fractal.

7. Pseudo-randomidad: El comportamiento de un sistema caótico puede parecer aleatorio, aunque en realidad es determinista. Esto lo hace útil en aplicaciones como la generación de números pseudo-aleatorios.

# Exponentes de Lyapunov

Los exponentes de Lyapunov son una herramienta crucial en el análisis de sistemas dinámicos, particularmente en el contexto de la teoría del caos. Estos exponentes permiten cuantificar la sensibilidad de un sistema a las condiciones iniciales, lo que desempeña un papel fundamental en la determinación de si un sistema es caótico o no. La idea central detrás de los exponentes de Lyapunov es que en un sistema caótico, las pequeñas variaciones en las condiciones iniciales resultan en trayectorias futuras extremadamente divergentes. 

Los exponentes de Lyapunov son valores numéricos que se calculan para cada dirección en el espacio de fase del sistema. Estos exponentes describen cómo se separan o acercan las trayectorias iniciales a medida que evolucionan en el tiempo. En sistemas con múltiples grados de libertad, se calcula un exponente de Lyapunov para cada dirección, proporcionando una imagen completa de la sensibilidad del sistema. 

Un exponente de Lyapunov positivo indica que las trayectorias se alejan entre sí, lo que es una característica distintiva de los sistemas caóticos. Por otro lado, un exponente negativo señala que las trayectorias se acercan entre sí, indicando un sistema estable y convergente. Cuando el exponente de Lyapunov es igual a cero, las trayectorias son paralelas y no muestran ni separación ni convergencia, lo que sugiere un sistema neutral o marginalmente estable, por otro lado si es positivo el sistema es caótico, finalmente si el exponente de Lyapunov es negativo, indica que las trayectorias se acercan entre sí, lo que es característico de un sistema estable y convergente.

El coeficiente de Lyapunov es una medida de caos del sistema dinámico y esta definido como:

*Si el sistema discreto $X_{t+1}$ es caótico, con exponente $\lambda$ Entonces, para muchos $X_0$ y para todo $\epsilon > 0$ pequeño y constante, siendo epsilon la diferencia entre condiciones iniciales*
$$
|X_t(X_0 + \epsilon) - X_t(X_0)| \backsim \epsilon e^{\lambda t}
$$
Esto para una $t$ grande, así mediante cálculos se puede llegar a que el exponente de Lyapunov esta definido como:

$$
\lambda = \lim_{t \rightarrow \infty} (\frac{ln(\frac{\partial f^t(x)}{\partial t})}{t})
$$

