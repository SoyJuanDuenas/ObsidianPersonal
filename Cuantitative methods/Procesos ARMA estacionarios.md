Los procesos ARMA estacionarios son  [[Procesos ARMA]] y [[procesos estacionarios]] al mismo tiempo, estos tienen diferentes características que vamos a enunciar a continuación, iniciaremos enunciando los diferentes

Los [[procesos ARMA]] (Autoregressive Moving Average) que son también [[procesos estacionarios]], a menudo abreviado como "proceso ARMA estacionario", es un tipo de [[time series models]] en el que se cumplen ciertas condiciones que hacen que la serie temporal exhiba propiedades de estacionariedad, lo que significa que sus propiedades estadísticas no cambian con el tiempo.
# Características

Un proceso ARMA estacionario se caracteriza por las siguientes propiedades:

1. **Media Constante:** La media de la serie temporal es constante a lo largo del tiempo. Esto significa que, en promedio, los valores de la serie no cambian a medida que avanzamos en el tiempo. La constancia de la media es una característica clave de la estacionariedad.

2. **Varianza Constante:** La varianza de la serie temporal es constante. Esto implica que la dispersión o la variabilidad de los valores de la serie no cambia a lo largo del tiempo.

3. **Función de Autocorrelación Limitada:** La función de autocorrelación de la serie (que mide la relación entre los valores de la serie en diferentes momentos en el tiempo) se desvanece rápidamente a medida que aumenta el retraso temporal. En otras palabras, la influencia de los valores pasados en los valores futuros disminuye con rapidez.
# Representación

Un proceso ARMA estacionario se puede representar de la siguiente manera:

$$Y_t = a_0 + a_1 X_{t-1} + a_2 X_{t-2} + \dots + a_p X_{t-p} + \varepsilon_t + \beta_1 \varepsilon_{t-1} + \beta_2 \varepsilon_{t-2} + \dots + \beta_q \varepsilon_{t-q}$$

Donde:
- $Y_t$ es el valor en el tiempo $t$.
- $a_0$ es una constante.
- $a_1, a_2, \dots, a_p$ son los coeficientes autorregresivos.
- $\varepsilon_t$ es el término de error en el tiempo $t$.
- $\beta_1, \beta_2, \dots, \beta_q$ son los coeficientes de promedio móvil.
- $p$ es el orden autorregresivo.
- $q$ es el orden de promedio móvil.

Los procesos ARMA estacionarios son utilizados comúnmente en el análisis de datos financieros, económicos, climáticos y en otros campos donde se requiere modelar y predecir series temporales. La estacionariedad es una suposición importante para aplicar modelos ARMA de manera efectiva.

# AR estacionarios

## AR(1) Estacionario

Sea un proceso AR(1)

$$Y_t = a_0 + a_1Y_{t-1} + \varepsilon_t$$
Para garantizar que AR(1) es un proceso estacionario, verificamos que las raíces unitarias del polinomío caracteristica se encuentren por fuera del circulo unitario $|z| > 1$.
