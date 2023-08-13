Sea $S$ un conjunto no-vacío. Una relación binaria $R$ sobre $S$ es un subconjunto no-vacío del [[producto cartesiano]] $S \times S$ donde cada elemento en la relación son [[pares ordenados]] del conjunto original.

Abusando de la notación, si $(x,y) \in R$, entonces expresaremos esta relación binaria como $xRy$
# Tipos de relaciones binarias

Para entender de manera adecuada los tipos de relaciones binarias es fundamental hacer uso del [[lenguaje lógico]], a continuación detallaremos los diferentes tipos de relaciones binarias y sus características.

- $R$ es una relación binaria reflexiva si para todo $x \in S$, $xRx$
- $R$ es una relación binaria irreflexiva si para todo $x \in S$, $x\not Rx$
- $R$ es una relación binaria simétrica si para todo $x,y \in S$, tales que $xRy$ se tiene que $yRx$
- $R$ es una relación binaria asimétrica si para todo $x,y \in S$, tales que $xRy$ se tiene que $y\not R x$
- $R$ es una relación binaria antisimétrica si para todo $x,y \in S$, tales que $xRy$ y $yRx$ se tiene que $y = x$
- $R$ es una relación binaria transitiva si para todo $x,y,z \in S$, tales que $xRy$ y $yRz$, entonces $xRz$
- $R$ es una relación binaria completa si para todo $x,y \in S$, se tiene que $xRy$ o $yRx$ (o ambos)
## Negación de los tipos de relaciones binarias

Por medio del [[lenguaje lógico]] podemos decir que no es un tipo de relación binaria, es decir todas son relaciones binarias de diferente tipo hasta que se demuestre lo contrario.

- **$R$ no es** una relación binaria reflexiva si existe algún $x\in S$ tal que $x\not R x$
- **$R$ no es** una relación binaria irreflexiva si existe algún $x\in S$ tal que $xRx$
- **$R$ no es** una relación binaria simétrica si existe algún $x,y\in S$ tal que $xR y$ y $y\not R x$
- **$R$ no es** una relación binaria asimétrica si existe algún $x,y\in S$ tal que $x R y$ y $yRx$
- **$R$ no es** una relación binaria transitiva si existe algún $x,y,z\in S$ tal que $x R y$ y $yRz$ pero $x\not R z$
- **$R$ no es** una relación binaria completa si existe algún $x,y\in S$ tal que $x\not R y$ y $y\not R x$
-
