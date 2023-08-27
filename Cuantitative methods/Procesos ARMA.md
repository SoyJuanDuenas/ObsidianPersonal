Un proceso ARMA (Autoregressive Moving Average) hace parte de los [[time series models]]. Este modelo combina dos componentes principales: el componente autorregresivo (AR) y el componente de promedio móvil (MA). Estos componentes son capaces de capturar la estructura y la dinámica de una serie temporal.  

# Componente Autorregresivo AR

En este componente, el valor actual de la serie temporal se modela como una combinación lineal de sus valores pasados, ponderados por coeficientes llamados parámetros autorregresivos. La idea detrás de la parte autorregresiva es que el valor actual depende de manera directa de sus valores anteriores. Matemáticamente, un proceso AR(p) se representa de la siguiente manera:

   $$Y_t = a_0 + a_1 Y_{t-1} + a_2 Y_{t-2} + \ldots + a_p X_{t-p} + \varepsilon_t$$

   Donde:
   - $Y_t$ es el valor en el tiempo $t$.
   - $a_0$ es una constante.
   - $a_1, a_2, \ldots, a_p$ son los coeficientes autorregresivos.
   - $\varepsilon_t$ es un término de error que representa la variabilidad no explicada por los valores pasados y que sigue un [[proceso de ruido blanco]].
# Componente de Promedio Móvil (MA)

En esta parte, el valor actual de la serie se modela como una combinación lineal de términos de error pasados, multiplicados por coeficientes llamados parámetros de promedio móvil. Esto refleja cómo los errores anteriores influyen en el valor actual. Matemáticamente, un proceso MA(q) se representa de la siguiente manera:

   $$Y_t = a_0 + \varepsilon_t + \beta_1 \varepsilon_{t-1} + \beta_2 \varepsilon_{t-2} + \ldots + \beta_q \varepsilon_{t-q}$$

   Donde:
   - $Y_t$ es el valor en el tiempo $t$.
   - $a_0$ es una constante que representa la media de la serie temporal $\mu$.
   - $\varepsilon_t$ es el término de error en el tiempo $t$ que sigue un [[proceso de ruido blanco]].
   - $\beta_1, \beta_2, \ldots, \beta_q$ son los coeficientes de promedio móvil.
   - $q$ es el orden de promedio móvil, es decir, cuántos términos de error pasados se incluyen en el modelo.

Un modelo ARMA(p, q) combina los componentes AR y MA para describir la serie temporal en términos de sus valores pasados y los errores pasados. La elección de los valores de $p$ y $q$ se basa en el análisis de datos y en técnicas estadísticas para encontrar el modelo que mejor se ajuste a los datos observados.