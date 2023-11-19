Los datos panel o datos longitudinales es un conjunto de datos donde cada individuo es observado durante dos o más periodos de tiempo. Estos individuos pueden ser hogares, personas, municipios, paises... etc

Los datos panel son útiles porque nos permiten controlar por factores especificos individuales no observados que no varian en el tiempo y que podrian causar sesgo de la variable omitida, además de obtener conclusiones a nivel de individuos y no solo a nivel poblacional como con la [[Combinación independiente de cortes transversales]]

# Efectos fijos / efectos inobservables

Supongamos el siguiente modelo: 

$$y_{it} = \beta_0 + \lambda_{0}(d2_t) + \beta_1x_{it} + a_{i} + u_{it}$$
donde: 

- $i$ denota el individuo
- $t$ denota el tiempo en el que se esta trabajando
- $d2_t$ Dummy que es 0 cuando t=1 y 1 cuando t=2
- $\beta_0$ intercepto para t = 1
- $\beta_0 + \lambda_0(d2_t)$ intercepto para t = 2
- $a_i$ efecto fijo, captura todos los efectos inobservables constantes en el tiempo que influyen en $y_{it}$
- $u_{it}$ como error idiosincrático.

Este modelo se puede expresar como:
$$y_{it} = \beta_0 + \lambda_{0}(d2_t) + \beta_1x_{it} + v_{it}$$
donde $v_{it} = u_{it} + a_i$ se denomina el error compuesto.

Para que los estimadores de MCO sean consistentes se requiere que el error compuesto no se correlacione con algún regresor por lo cual ni el error idiosincratico ni el efecto fijo se debe correlacionar con el regresor, tal que:

$$corr(u_{it}, x_{it}) = 0$$
$$corr(a_{it}, x_{it}) = 0$$
# Ecuación en primera diferencia

Sin embargo, usualmente la razón principal para recopilar datos panel es permitir que el efecto no observado $a_{it}$ se correlacione con las variables explicativas (controlar por efectos no observados), para lograr esto dado que el efecto no observado es constante en el tiempo debemos diferenciar. Tal que:

$$ y_{i1} = \beta_0 + \beta_1x_{i1} + a_{i} + u_{i1}$$
$$y_{i2} = (\beta_0 + \lambda_{0}) + \beta_1x_{i2} + a_{i} + u_{i2}$$
$$y_{i2} - y_{i1} = (\beta_0 + \lambda_{0}) + \beta_1x_{i2} + a_{i} + u_{i2} - \beta_0 - \beta_1x_{i1} - a_{i} - u_{i1}$$
$$\Delta y_i = \delta_0 + \beta_1(x_{i2} - x_{i1}) + (u_{i2} - u_{i1})$$
Lo cual nos lleva finalmente a la forma:
$$\Delta y_i = \delta_0 + \beta_1 \Delta x_i + \Delta u_i$$
En esta forma tenemos una [[Combinación independiente de cortes transversales]] solo que cada variable se encuentra diferenciada,  $\beta_1$ es denominado estimador en primera diferencia, aquí es muy importante que $(x_{i2} - x_{i1}) \neq 0$ es decir que la regresora cambie en el tiempo en cantidades diferentes (no se puede incluir constante como género o raza ni edad)

# Data panel para T periodos

El modelo de efectos fijos para T periodos está dado por la ecuación:
$$y_{it} = \delta_1 + \sum_{j = 2}^{T} \delta_{j}(dj_t) + \sum_{k = 1}^{K}\beta_{k}x_{itk} +  a_i + u_{it}$$

donde $t = 1, \dots , T$

Al introducir las variables dummies, el modelo va a variar para cada $i$, entonces diremos que para cada $i$ el modelo es:

$$y_{it} = \sum _{k = 1}^{K} \beta_k x_{itk} + a_i + u_{it}$$

## Ecuación en primera diferencia para T periodos

En este caso la ecuación en primera diferencia se obtiene restando el periodo uno del periodo dos, el periodo dos del periodo tres y así sucesivamente hasta restar el periodo T - 1 del periodo T, por lo cual la ecuación en primeras diferencias será de la forma:

$$\Delta y_{it} = \alpha_0 + \sum_{j = 3}^{T} \alpha_j(dj_t) + \sum_{k=1}^{K} \beta_{k} \Delta x_{itk} + \Delta u_{it}$$

