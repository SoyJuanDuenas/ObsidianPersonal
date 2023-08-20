Sea $S$ un conjunto no-vacío. Una relación binaria $R$ sobre $S$ es un subconjunto no-vacío del [[producto cartesiano]] $S \times S$ donde cada elemento en la relación son [[pares ordenados]] del conjunto original.

Abusando de la notación, si $(x,y) \in R$, entonces expresaremos esta relación binaria como $xRy$
# Tipos de relaciones binarias

Para entender de manera adecuada los tipos de relaciones binarias es fundamental hacer uso del [[lenguaje lógico]], a continuación detallaremos los diferentes tipos de relaciones binarias y sus características.

- $R$ es una relación binaria reflexiva si para todo $x \in S$, $xRx$
	Todo lo que está en $S$ debe en $R$ estar relacionada consigo misma
- $R$ es una relación binaria irreflexiva si para todo $x \in S$, $x\not Rx$
	Todo lo que está en $S$ no puede estar en $R$ relacionada consigo misma
- $R$ es una relación binaria simétrica si para todo $x,y \in S$, tales que $xRy$ se tiene que $yRx$
	Si en $R$ hay una relación, debe estar esa misma relación en sentido opuesto
- $R$ es una relación binaria asimétrica si para todo $x,y \in S$, tales que $xRy$ se tiene que $y\not R x$
	si en $R$ hay una relación, no puede estar esa relación en sentido opuesto
- $R$ es una relación binaria antisimétrica si para todo $x,y \in S$, tales que $xRy$ y $yRx$ se tiene que $y = x$
	preguntarle a pacho jajan't
- $R$ es una relación binaria transitiva si para todo $x,y,z \in S$, tales que $xRy$ y $yRz$, entonces $xRz$
- $R$ es una relación binaria completa si para todo $x,y \in S$, se tiene que $xRy$ o $yRx$ (o ambos)
	todas las relaciones de $S$ deben estar conectadas de algún modo en $R$ 
## Negación de los tipos de relaciones binarias

Por medio del [[lenguaje lógico]] podemos decir que no es un tipo de relación binaria, es decir todas son relaciones binarias de diferente tipo hasta que se demuestre lo contrario.

- **$R$ no es** una relación binaria reflexiva si existe algún $x\in S$ tal que $x\not R x$
- **$R$ no es** una relación binaria irreflexiva si existe algún $x\in S$ tal que $xRx$
- **$R$ no es** una relación binaria simétrica si existe algún $x,y\in S$ tal que $xR y$ y $y\not R x$
- **$R$ no es** una relación binaria asimétrica si existe algún $x,y\in S$ tal que $x R y$ y $yRx$
-  Como se niega una antisimetrica ?
- **$R$ no es** una relación binaria transitiva si existe algún $x,y,z\in S$ tal que $x R y$ y $yRz$ pero $x\not R z$
- **$R$ no es** una relación binaria completa si existe algún $x,y\in S$ tal que $x\not R y$ y $y\not R x$
## relaciones entre tipos

Ahora mostraremos como entre diferentes tipos de relaciones binarias se pueden crear nuevos tipos de relaciones binarias, adicional de como estos pueden llegar a estar conectados

- Toda relación completa es una relación reflexiva
- $R$ es una relación binaria racional si es una relación completa y transitiva
- $R$ es una relación binaria de orden parcial si es una relación reflexiva, transitiva y antisimétrica
- $R$ es un orden estricto si es una relación asimétrica y transitiva
# Ejemplos:

$$
S = \{x,y,z\}; R = \{(x,y), (y,x),(x,z)\}
$$
- $R$ no es una relación reflexiva dado que no existe algún $x,y,z$ que se relacione consigo mismo
- $R$ es una relación irreflexiva dado que para todo $x,y,z$ no existe alguno que se relacione consigo mismo
- $R$ no es una relación simétrica dado que existe algún $xRz$ y $z \not R x$
- $R$ no es una relación asimétrica dado que existe algún $xRy$ y $yRx$
- #Creo que $R$ no es una relación antisimetrica dado que 
- $R$ no es una relación transitiva dado que existe algún $yRx$ y $xRz$ pero no $yRz$
- $R$ no es completa porque existe algún $y\not Rz$ y $z\not R y$

$$
S = \{x,y,z\}; \tilde{R} = \{(x,x)\}
$$
- $\tilde{R}$ no es reflexiva, dado que existe algún $y\not Ry$
- $\tilde{R}$ no es irreflexiva dado que existe algún $xRx$
- $\tilde{R}$ es simétrica dado que la única forma de cumplir $aRb$ es $a=b=x$
- $\tilde{R}$ es transitiva dado que la manera en que se cumple que $aRb$ y $bRc$ entonces $aRc$ es que $a=b=c=x$

$$
S = \{\emptyset, \{1\}, \{3,5\} \}; R = \{(\emptyset, \emptyset), (\emptyset,\{1\}), (\emptyset, \{3,5\}), (\{1\},\{1\}), (\{3,5\},\{3,5\})\}
$$
- $R$ es reflexiva dado que para todo elemento de $S$ hay un $aRa$
- $R$ no es irreflexiva dado que existe al menos un elemento que se relacione consigo mismo
- $R$ no es simétrica dado que hay algún $\emptyset R \{1\}$ y $\{1\}\not R \emptyset$
- $R$ es asimétrica dado que para todo $aRb$, $b\not R a$ 
- ni idea si es antisimétrica
- $R$ es transitiva porque no hay ninguna pareja que cumpla el antecedente pero no el consecuente
- $R$ no es completa dado que $\{1\} \not R \{3,5\}$ y $\{3,5\} \not R \{1\}$ 

## Tarea

Describa una relación simétrica, completa y no transitiva

$$
S = \{x,y,z\}; R = \{(x,y),(y,z),(y,x),(z,y)\}
$$
