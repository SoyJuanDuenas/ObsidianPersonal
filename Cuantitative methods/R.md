R is a free and open-source [[programming language]] and statistical development environment that allows anyone to download, use, and modify it. Consequently, it has a large community and well-documented functionalities and [[packages]]. R is an [[object-oriented language]], which means that data is organized into objects that can be manipulated and analyzed. Additionally, R is accompanied by a graphical user interface called RStudio, which facilitates working with the language and enables easy data creation and visualization.

The versatility of R permits various types of analyses, including [[descriptive statistics]], [[bayesian statistics]], [[state-space models]], and more. Notably, R can be utilized for [[macroeconometrics]], [[microeconometrics]], [[financial econometrics]], [[impact evaluation]], [[bayesian econometrics]], [[spatial econometrics]], and other analyses.
# RStudio

RStudio provides a graphical user interface (GUI) that makes working with R easier, thus making it more accessible for users who are not familiar with command-line programming.

Upon entering RStudio, we will encounter four main panels:

![[Vista General RStudio.png]]
1. **Editor:** In the editor, we will place the code and execution commands.
2. **Console:** Here, we will see the results or outputs of the code.
3. **Workspace:** In this panel, we can view the command history we have used, different variables, datasets, [[objects]], [[functions]], and other elements we have declared.
4. **Files / Plots / [[packages]]** Here, we can visualize the plots generated in the code, installed [[packages]], files from our PC, among other things.

Usually, most of the work in R is done in the first panel. Here, we are going to program in R.  

# Comments

It is a good practice to comment our code, which means adding non-executable text that explains what our code is doing. This will help us and other people understand and correct our work in the future. To comment the code, we use `#`, and any text following the pound sign will not be executed.

```{r}
#Esto es un comentario
```

# [[packages]] and Workspace Cleaning

R always keeps different variables, datasets, and other [[objects]] stored in memory. Therefore, it is a good practice to clean our workspace at the beginning of each code. We can do this with the following command:

```{r}
remove(list = ls())
```

Since R is an open-source language, users can create [[packages]] to facilitate or perform new operations that are not available in the base R. However, to use these [[packages]], we need to install and then activate them. The installation is only done once, while the activation should be done again each time we open RStudio. It is a good practice to activate all the required [[packages]] in the first lines of the code.

```{r}
#| output: false
options(repos = c(CRAN = "http://cran.rstudio.com"))
install.packages("dplyr")
install.packages("ggplot2")
```

```{r}
#| output: false
library(dplyr)
library(ggplot2)
```

The first code block removes all objects from the workspace, effectively cleaning it. The following two code blocks handle the installation and activation of the `dplyr` and `ggplot2` [[packages]], respectively, which are common [[packages]] used for data manipulation and visualization in R. The `#| output: false` lines are comments that tell the code not to show the output of these commands when they are executed.
# Arithmetic Operations in R

R includes several arithmetic operators used to perform mathematical operations. The arithmetic operators are:

- `+`: Adds two numbers
- `-`: Subtracts two numbers
- `*`: Multiplies two numbers
- `/`: Divides two numbers
- `**`: Raises a number to a power

# Logical and Comparison Operators in R

Logical operators are used to combine logical expressions and produce a true or false result. Additionally, comparison operators can be used to create logical expressions. The logical and comparison operators for vectors and matrices are as follows:

```R
a = 2
# Elements greater than or equal to j in the vector
a >= 4

# Elements less than or equal to j in the vector
a <= 4

# Elements equal to j in the vector
a == 4

b = 2
# Elements different from i in the vector
b != 6

# Two true statements: "&"
a >= 1 & b == 3 # Remember that & represents logical "and"

# At least one is true: "|"
a >= 1 | b == 3 # Remember that | represents logical "or"

# Negation: "!"
!a < 0 # a is not less than zero
```

# NA and NaN

When the code reports an NA value, it indicates a missing value, i.e., empty data. On the other hand, when we have a NaN (not a number), it means that the result of the operation cannot be calculated as it is indeterminate.

# Variables and [[objects]] types in R

We define a variable as a "container of information" in which we can "store" different [[objects]]. Generally, variable names are written in lowercase, without spaces, accents, commas, periods, question marks, or any other character except underscores. In R, we can declare variables using either `<-` or `=`. For notation in this book, we will use only the equal sign.

```R
variable_name <- "Value of the variable"
variable_name = "Value of the variable"
```

To view our variable in the console (Panel #2), we can call it again, use the `print` [[function]], or use a semicolon and call the [[function]] on the same line.

```R
variable_name
print(variable_name)
variable_name = "Value of the variable"; variable_name
```

The objects we store in variables can be of different types, and depending on this, the way of storing them changes. In R, the following types of [[objects]] exist:

- **Numeric:** Data that consists of numbers, which can be continuous (allow decimals) or discrete (do not allow decimals).
- **Logical:** Can only have two values, `True` or `False`.
- **Character:** Strings of characters, i.e., words.
- **Complex:** Objects that belong to the complex plane.

```R
numeric_object = 3
logical_object = FALSE
character_object = "Hello, World"
complex_object = 1+0i
```

To verify the type or class of an [[objects]], we can use the `class` [[function]]. It may be necessary to convert an object from one type to another; for this, we use the appropriate [[function]]:

```R
x = 1
class(x)

as.numeric(x)
as.logical(x)
as.character(x)
```

To perform operations between variables, ensure that the variables are of numeric type and perform the operation:

```R
a = 5
b = 7

c = a + b
c
```

# [[data structures]] in R

Una colección puede contener varios objetos o elementos en determinado orden o estructura, Las colecciones son fundamentales y se utilizan para almacenar y manipular datos. se organizan por su dimensión (1ra, 2da, varias dimensiones) y si son homogeneas (todos los objetos deben ser del mismo tipo) o heterogeneas, 

We will detail the main [[data structures]] used in R.

Sure! Here's the translation of the text:

## Vectors

Vectors are structures of homogeneous dimensionality. These are mathematical entities used to store finite objects of a specific type. To create vectors in R, we use the `c()` command. Vectors allow us to perform operations on multiple data simultaneously without resorting to loops. There are four types of vectors classified according to the type of data they contain:

- **Numeric:** In R, numeric vectors are numeric by default (they can have decimal values).
- **Character:** Vector of characters, also known as strings.
- **Logical:** Can only take three possible values: `TRUE`, `FALSE`, and `NA`. Logical vectors are usually the result of logical or comparison operations.
- **Integer:** In R, numeric vectors are numeric by default (they can have decimal values). To create an integer (a whole number without decimals), we add the letter 'L' after the number.

```{r}
numeric_vector = c(25, 5, 3, 6, 3, 6)
character_vector = c("Hello", "world")
logical_vector = c(FALSE, TRUE, FALSE, TRUE)
```

To check the type of vector, we use:

```{r}
typeof(logical_vector)
```

Since vectors can only store one type of data, if we introduce different types of data, the vector will automatically convert these data to maintain a single data type, following this order:

$$
\text{logical < integer < double < character}
$$

Where the types on the right are more heavily weighted than those on the left.

```{r}
y <- c(1.7, "a")   ## character
y <- c(TRUE, 2)    ## numeric
y <- c("a", TRUE)  ## character
```

We can create vectors with specific characteristics efficiently, for example:

```{r}
# Create a sequence vector from 1 to 15.
Days = 0:15; Days

# Create a sequence vector that advances by j units: seq(a, b, j)
Measurement = seq(1, 5, 0.5); Measurement

# Create a vector where the objects are repeated n times: rep(object, n)
Numeric = rep(1, 10); Numeric

# Create a vector with repetitions
Dummy = c(rep(0, 5), rep(1, 10), rep(0, 5)); Dummy
```

To concatenate vectors, we simply use:

```{r}
vector_a = c(2, 54, 3)
vector_b = c(3, 7, 8)
vector_c = c(vector_a, vector_b); vector_c
```

Operations with vectors work similarly to operations with variables. In the end, we are still operating on variables, but in this case, the variables contain a vector of values. The vectors must be of the same length or multiples of each other for operations to work. If they are of the same length, the operation will be performed element-wise; if they are multiples, the operation will be repeated for different vectors, like this:

```{r}
# Element-wise operation
vector_a = c(2, 54, 3)
vector_b = c(3, 7, 8)
vector_c = vector_a + vector_b; vector_c

# Operation between multiples
vector_a = c(2, 54, 3, 4, 8, 5)
vector_b = c(3, 7, 8)
vector_c = vector_a + vector_b; vector_c
```

We can perform descriptive statistics on vectors using the `summary` function, among other possible methods for vector class:

```{r}
summary(vector_a)
```

Other possible methods for vectors include:

```{r}
# Describe which elements are unique in the vector
unique(vector_a)

# Sort elements in ascending order
sort(vector_a)  

# Get the ordered position from the smallest to the largest
order(vector_a) 

# Sort elements in descending order
sort(vector_a, decreasing = TRUE)       
```

Sometimes we want to access a specific part of the vector or even a single element. For this, we use square brackets \[ \]. Unlike Python, R is 1-based, so elements are counted starting from 1.

```{r}
v = c("one", "two", "three", "four")
new_vector = v[c(1, 3, 2)]; new_vector
```

In the above line of code, we created a character vector with numbers from one to four. Then, we saved in a vector called `new_vector` the first, third, and second elements of the vector `v`.

Negative values remove elements from the specified positions:

```{r}
v = v[c(-2)]; v
```

In the above line of code, we removed the second element from vector `v` and overwrote the vector with the changes.
### [[matrix]]

A matrix is a two-dimensional collection of data consisting of elements of the same type organized in rows and columns (bidimensional and homogeneous). It can be represented as a table or grid of numbers or values. Each element in the matrix is identified by its position determined by the row and column number.

To create matrices in R, we can do it directly or from previously created vectors. To create matrices directly, we use:

```{r}
MAT1 = matrix(1:10, nrow = 5, byrow = TRUE); MAT1 
MAT2 = matrix(10:19, ncol = 5, nrow = 2, byrow = FALSE); MAT2
```

Where the first parameter corresponds to the values to be used to fill the matrices. This interval must be a multiple of the number of rows or columns we want to create. The second parameter determines if we want to create the matrix by rows (`byrow = TRUE`) or by columns (`byrow = FALSE`).

Now, if we want to create matrices from previously established vectors, we use the following code:

```{r}
a = c(1, 4, 5, 7, 9, 7, 10, 6, 5, 7, 9)
b = c(3, 4, 6, 8, 2, 3, 11, 1, 2, 5, 6)
MAT3 = cbind(a, b); MAT3
MAT4 = rbind(a, b); MAT4 
```

As we can see, when using vectors, we can also create matrices by rows or by columns.

Matrices have different ways of being operated compared to scalars or constants. Let's detail each of the main operations:

```{r}
# Scalar-matrix addition
MAT1 + 10

# Matrix-matrix addition
MAT3 + t(MAT4)

# Scalar-matrix multiplication
MAT3 * 10
```

We can also create special matrices:

```{r}
# Transpose of a matrix: t() 
t(MAT1) 

# Identity matrix: diag()
diag(5)

# Diagonal matrix: diag()
Mat_diag = diag(1:10)
```

Finally, we'll calculate matrix multiplication, which is not performed element-wise but through a different process. We will also calculate the inverse of a matrix and its determinant
$$
Ax = b
$$

$$
3x + 2y = 5
$$

$$
x-y = 0
$$

el cual expresado matricialmente se expresa como:

$$
\begin{bmatrix}
 3 & 2 \\
 1 & -1 \\
\end{bmatrix}
\begin{bmatrix}
 x \\
 y \\
\end{bmatrix}
=
\begin{bmatrix}
 5\\
 0\\
\end{bmatrix}
$$

Podemos resolver el sistema de ecuaciones en R del siguiente modo:

```{r}
A = matrix(c(3,2,1,-1), ncol = 2, byrow = TRUE)
b = c(5, 0)
solve(A, b)
```

Para acceder a elementos especificos de la matriz debemos hacer uso del indice en formato (x,y) tal que sea (fila, columna)

```{r}
MAT2
#Mostrar el elemento ij de la matriz: MAT[i,j]
MAT2[2,1]
MAT2[1,2]
```

podemos hacer esto tambien para mostrar solo una fila o solo una columna de la matriz

```{r}
MAT2
#Mostrar los elementos de la fila i: MAT[i,]
MAT2[1,]

#Mostrar los elmentos de la columna j: MAT[,j]
MAT2[,1]
```

Para mejor entendimiento de nuestra matriz podemos cambiarle los nombres a las filas y las columnas, esto nos facilitará el trabajo posterior.

```{r}
rownames(MAT1) = c("a","b","c","d","e")
colnames(MAT1) = c("f","g")
MAT1
```

Si queremos añadir columnas y filas a nuestras matrices creadas con anterioridad podemos emplear las funciones `cbind()` y `rbind()` respectivamente

```{r}
MAT1=matrix(1:10,nrow = 5,byrow = TRUE)
MAT1 = rbind(MAT1, c(30,30));MAT1
```

```{r}
MAT1=matrix(1:10,nrow = 5,byrow = TRUE)
MAT1 = cbind(MAT1, c(30,30,30,30,30));MAT1
```

Para eliminar filas usaremos \[-i,\] mientra que para eliminar columnas utilizaremos la notación \[ , -j\]

```{r}
MAT1 = MAT1[-5,]; MAT1
```

```{r}
MAT1 = MAT1[,-3]; MAT1
```

### Listas

### Dataframes

## PENDIENTES

Completar listas y dataframes, pasar los de titulo 2 a titulo 1 y los de titulo 3 a titulo 2 y hacer de los diferentes metodos de las estructuras de datos titulos 3, cambiar a str las matrices especiales y disminuir su dimensionalidad.
