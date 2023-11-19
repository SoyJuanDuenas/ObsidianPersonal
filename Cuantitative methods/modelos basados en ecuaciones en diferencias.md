Un modelo basado en [[ecuaciones en diferencia]] es una herramienta matemática utilizada para describir el comportamiento de sistemas dinámicos discretos en el tiempo. Estas ecuaciones son una extensión de las ecuaciones diferenciales, que describen cómo las variables cambian en términos de sus derivadas con respecto al tiempo en sistemas continuos.

Los modelos basados en ecuaciones en diferencias pueden volverse más complejos al incorporar múltiples variables, restricciones y relaciones entre variables. Estos modelos son útiles para simular y predecir el comportamiento de sistemas discretos en el tiempo y para analizar cómo diferentes factores afectan el desarrollo de esos sistemas a lo largo del tiempo.
# Ecuación lineal

Un ejemplo sencillo de un modelo basado en [[ecuaciones en diferencia]] es el modelo de crecimiento poblacional discreto. Supongamos que tienes una población de organismos que se reproduce cada año. La ecuación en diferencias podría verse así:

$$X_{t+1} = r  X_{t}$$

Donde:
- $X_{t}$ es la población en el tiempo t.
- $r$ es la tasa de crecimiento.
- $X_{t+1}$ es la población en el tiempo t+1.

Esta ecuación en diferencias establece que la población en el próximo año (t+1) es igual a la población actual (t) más el incremento proporcional al tamaño actual de la población multiplicado por la tasa de crecimiento.

Al iterar nos podemos encontrar con que la solución explicita a este modelo es:
$$X_{t+1} = rX_t$$
$$X_{t+2} = rX_{t+1} = r(rX_t) = r^2(X_t)$$
$$X_{t+3} = rX_{t+2} = r(r^2X_t) = r^3{X_t}$$
Lo cual generalizando obtenemos que:
$$X_t = r^{t}X_0$$
llevando a la conclusión de que

- Si r < 1, la población se extingue con decrecimiento exponencial
- Si r = 1, la población se mantiene estable en $X_0$
- Si r > 1, la población explota con crecimiento exponencial

Esto ultimo recordando las propiedades de las [[sucesiones]], especialmente la sucesión de la forma: $$\{r^n\}_{n=1}^{\infty}$$
# Ecuación de modelo poblacional logística (No lineal)

Supongamos la siguiente ecuación no lineal en la cual demostramos las complicaciones que puede presentar una no-linealidad.

$$X_{t+1} = rX_t(1 - x_t)$$
$$X_{t+1} = rX_t - rX_{x}^{2}$$
con r > 0, tenemos que el termino $(1 - X_t)$ contrae el crecimiento de la población que si no estuviera, crecería o decrecería exponencialmente como la ecuación lineal.

El más simple comportamiento a investigar en las [[ecuaciones en diferencia]] son los equilibrios que se definen cuando $F(X^*) = X^*$, en el caso de la ecuación logística resultan de resolver.
$$X^* = rX^*(1-X^*)$$
Los equilibrios son:
- $X^* = 0$
- $X^* = 1 - (1/r)$ >0

Al igual que el modelo anterior dependiendo del valor de R el equilibrio y la dinámica va a ser diferente.

Sí:
- r < 1, la población se extinguirá ($X^* = 0$)
- r > 1, la población se ajustará a un nivel fijo $X^*$ o fluctuará a lo largo de una serie de booms y depresiones poblacionales

![[Pasted image 20230814200147.png]]
Siendo *Growth Rate* igual a r.

cuando $r$ es lo suficientemente grande, nos damos cuenta que hay un limite, que hay un freno poblacional en $(1-X_t)$ que generan los comportamientos 2-ciclo y 4-ciclo que se pueden con $r = 3$ y $r = 3.5$ respectivamente. pero es una regularidad, pero que no es una convergencia y por ende tampoco un estado estacionario. 

Sin embargo, la dinámica de la ecuación logística es más complicada que eso: puede producir fenómenos de [[alta sensibilidad a las condiciones iniciales]] ($X_0$) manteniendo r constante y por ende comportamientos con k-ciclos.

![[Pasted image 20230814202352.png]]

esto empieza a surgir después de $r > 3.57$ ([[valor de Feigenbaum]]) parece una dinámica aleatoria pero es determinística.

la primera grafica tenemos que $X_0 = 0.3$ y $Y_0 = 0.301$ mientras que la segunda uc$X_0 = 0.3, Y_0 = 0.300001$ entre menor sea la diferencia de la condición inicial, más se va a demorar en diferenciarse las series.

La [[alta sensibilidad a las condiciones iniciales]] se puede evidenciar en el mediano y largo plazo. Dado que las variables económicas la mayoría presentan esta condición, no puede predecirse variables económicas en el mediano y largo plazo.

Lo que hace que se empiecen a diferenciar a partir de determinado momento las series es porque en estas dinámicas no lineales se presenten [[positive feedbacks]] que son pequeñas acumulaciones de efectos que llegan a un punto limite y generan la diferencia. Es por esto que todas las variables economicas tienen [[incertidumbre fundamental]] ( George Shackle), sin embargo hay algunas [[time series models]] que presentan [[ergodicidad]] las cuales nos permiten predecir ciertos promedios e intervalos en el mediano y largo plazo.

Se buscan regularidades en vez de equilibrios dado que en las regularidades se pueden encontrar estructuras fractales, un ejemplo en economía es como en ciertas variables por ejemplo en ingresos la distribución es la misma en LA como en Bogotá como lo trabajo Luis Betancur en su trabajo *Introduction to Urban Science, Evidence and Theory of Cities as Complex Systems*. también estos fénomenos se pueden presentar en [[time series models]].


![[Pasted image 20230815163958.png]]

Como nos podemos dar cuenta en ciertas regiones se muestran repentinos y dramáticos cambios, a estos les denominaremos [[bifurcaciones]].

diremos que es condición suficiente la existencia de un 3-ciclo en un sistema para que ese sistema se presenten [[sistemas dinámicos caóticos]]






