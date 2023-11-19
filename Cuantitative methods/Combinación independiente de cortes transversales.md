Una combinación independiente de cortes transversales es un conjunto de datos obtenidos mediante un muestreo aleatorio de una población grande en distintos puntos del tiempo.

A diferencia de los [[datos panel]] el termino de error en una combinación independiente de corte transversal no se correlaciona para distintas observaciones. Es decir, las variables de las diferentes encuestas son iguales pero los individuos a los cuales se les aplica esta encuesta son diferentes pero que pertenecen a un mismo grupo poblacional. Otra diferencia entre estas dos metodologias es que en la combinación independiente de cortes transversales no podemos hablar de cambios o prevalencias de atributos poblacionales.

Usualmente encontramos este tipo de datos en encuestas llevadas a cabo periodicamente algunos ejemplos colombianos pueden ser la GEIH

En la combinación independiente de cortes transversales debemos usar [[variables dummies]] para diferenciar el periodo en el cual estamos trabajando entre el periodo base y el periodo a comparar.
# Ejemplo

Usando datos para 550 personas en 1978 y un grupo diferente de 534 personas en 1985 se desea estimar el siguiente modelo de regresión para determinar si la rentabilidad de la educación
y las diferencias de salario por género han cambiado de 1978 a 1985:

$$\log{(wage)} = \beta_{0} + \lambda_{0}(y85) + \beta_{1}(educ)  + \lambda_{1}(y85)(educ) +  \beta_{2}(exper) +  \beta_{3}(exper)^{2} + \beta_{4}(union) + \beta_{5}(female) + \lambda_{5}(y85)(female) + u $$
donde:

- $wage$ es el salario por hora
- $educ$ son los años de educación
- $exper$ son los años de experiencia
- $union$ variable binaria que explica la (o la no ) afiliación de una persona a un sindicato
- $y85$ dummy que es igual a 1 si el año es igual a 1985 y 0 si es igual a 1978
- $\beta_{0}$ intercepto del año 1978
- $\beta_{0} + \lambda_{0}(y85)$ intercepto del año 1985
- $\beta_{1}$El impacto de la educación en 1978
- $\beta_{1} + \lambda_{1}(educ)$ el impacto de la educación en 1985
- $\beta_{5}$ diferencia en el ingreso entre mujeres y hombres en 1978
- $\beta_{5} + \lambda_{5}(y85)(female)$ diferencia en el ingreso entre mujeres y hombres en 1985


