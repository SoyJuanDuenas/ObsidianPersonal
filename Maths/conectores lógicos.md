Un operador lógico nos permite unir diferentes [[proposición]] para crear proposiciones más complejas, estos operadores lógicos tienen propiedades que interactuan con los valores de verdad de las [[proposición]], debemos tener claro las tablas de verdad de cada una de estos operadores lógicos para obtener el valor de verdad de la nueva proposición.

Los operadores lógicos son los siguientes: 
## Negación

Dada una proposición $\alpha$, la negación $\neg \alpha$ = $\neg (\alpha)$ corresponde a afirmaciones del tipo:

- No es cierto que $\alpha$
- No es verdad que $\alpha$
- No es el caso que $\alpha$
- No se tiene que $\alpha$
- Es falso que se tenga $\alpha$
### Ejemplos de negación

- No es cierto que a pepe le gustan los carros
- Es falso que la lógica estudia métodos para entender cuando un argumento es valido o no
### Tabla de verdad de la negación

Cuando la proposición sea verdadera, su negación es falsa. Cuando la proposición sea falsa, su negación es verdadera.


![[Pasted image 20230809154202.png]]
## Conjunción

Sea $\alpha$ y $\beta$ proposiciones, la conjunción $\wedge$, de $\alpha$  y $\beta$ corresponde a afirmaciones del tipo:

- $\alpha$ y $\beta$ 
- Es el caso que $\alpha$ y $\beta$
- Se tiene que $\alpha$ y $\beta$
- $\alpha$ pero $\beta$ (el "pero" se usa para indicar que $\beta$ tiene un sentido negativo respecto de $\alpha$)

La conjunción de $\alpha$ y $\beta$ están denotadas por:

$$
\alpha \wedge \beta
$$
$$
(\alpha) \wedge (\beta)
$$
### Ejemplos de conjunción

- Pepe es un gato pardo y Raffles es un perro labrador.
- A Juan le gusta ver películas pero José prefiere escuchar música.
### Tabla de verdad de la conjunción

La conjunción es verdadera únicamente cuando $\alpha$ y $\beta$ son verdaderas

![[Pasted image 20230809161645.png]]

## Disyunción

Sea $\alpha$ y $\beta$ proposiciones, la disyunción $\lor$, de $\alpha$  y $\beta$ corresponde a afirmaciones del tipo:

- $\alpha$ o $\beta$ 
- Es el caso que $\alpha$ o $\beta$
- Se tiene que $\alpha$ o $\beta$
- o bien $\alpha$,  o bien $\beta$

La disyunción de $\alpha$ y $\beta$ están denotadas por:

$$
\alpha \lor \beta
$$
$$
(\alpha) \lor (\beta)
$$
### Ejemplos de disyunción

- Pepe es un gato pardo o Raffles es un perro labrador.
- O bien a Juan le gusta ver películas o José prefiere escuchar música.
### Tabla de verdad de la disyunción

La disyunción es verdadera cuando alguna o ambas proposiciones son verdaderas.

![[Pasted image 20230809163019.png]]
## Condicional

El condicional esta conformado por dos tipos de proposiciones un antecedente $\alpha$ y un consecuente $\beta$  que sin que implique una causalidad, esta corresponde a afirmaciones del tipo:

- $\alpha$ implica $\beta$
- $\beta$, si $\alpha$
- si $\alpha$, entonces $\beta$
- si $\alpha$, $\beta$
- $\alpha$ solo si $\beta$
-  $\alpha$ es condición suficiente para $\beta$
- $\beta$ es condición necesaria para $\alpha$

El condicional entre $\alpha$ y $\beta$ esta denotado por:

$$
\alpha \rightarrow \beta
$$
$$
(\alpha) \rightarrow (\beta)
$$
### Ejemplos de condicional 

- Si amas a Dios entonces amas a tu hermano
- Que el agua alcance una temperatura de 100° es condición suficiente para que hierva

### Variantes del condicional

Si consideramos el condicional $(\alpha) \rightarrow (\beta)$ algunas variantes que debemos tener en cuenta son las siguientes:
#### La reciproca

$$
(\beta)\rightarrow (\alpha)
$$
#### La contrarrecíproca

$$
(\neg(\beta))\rightarrow (\neg(\alpha))
$$
#### La contraria

$$
(\neg(\alpha))\rightarrow (\neg(\beta))
$$
### Ejemplos de variantes del condicional

Suponga las siguientes proposiciones

- $\alpha$: "Hoy hay clase de Fundamentos de Matemáticas"
- $\beta$: "Hoy es martes"

por lo cual diremos que:

- $(\alpha) \rightarrow (\beta)$: "Si hoy hay clase de Fundamentos de Matemáticas, entonces hoy es martes"
- $(\beta)\rightarrow (\alpha)$: "Si hoy es martes, entonces hoy hay clase de Fundamentos de Matemáticas"
- $(\neg(\beta))\rightarrow (\neg(\alpha))$: Si hoy no es martes, entonces hoy no hay clase de Fundamentos de Matemáticas
- $(\neg(\alpha))\rightarrow (\neg(\beta))$: Si hoy no hay clase de Fundamentos de Matemáticas, entonces hoy no es martes

### Tabla de verdad de la condicional

decimos que el condicional es falso únicamente cuando el antecedente es falso y el consecuente verdadero, es decir. De una verdad no podemos concluir una falsedad

![[Pasted image 20230809191004.png]]

## Bicondicional

Sea $\alpha$ y $\beta$ proposiciones, la bicondicional $\leftrightarrow$, de $\alpha$  y $\beta$ corresponde a afirmaciones del tipo:

- $\alpha$ si y sólo si $\beta$
- $\alpha$ es equivalente a $\beta$
- $\alpha$ implica $\beta$ y $\beta$ implica $\alpha$
- $\alpha$ es condición suficiente y necesaria para $\beta$

Denotamos el bicondicional como:

$$
(\alpha) \leftrightarrow (\beta)
$$
### Ejemplos del bicondicional

- Que un entero no sea par es equivalente a que dicho entero sea impar
### Tabla de verdad del bicondicional

decimos que el bicondicional es verdadero donde el antecedente y el consecuente toman el mismo valor de verdad
![[Pasted image 20230809192319.png]]

