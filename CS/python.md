Python is an interpreted, [[object-oriented language]], high-level, slow, easy-to-learn [[programming language]] commonly used in data analysis including [[descriptive statistics]], [[bayesian statistics]], [[state-space models]], [[time series models]], [[data panel]] and more. Notably, Python can be utilized for [[macroeconometrics]], [[microeconometrics]], [[financial econometrics]], [[impact evaluation]], [[bayesian econometrics]], [[spatial statistics]], [[machine learning]], [[deep learning]], [[computer vision]], and other analyses. making it a multiparadigm language.

Python can be executed in two main ways, either from a text editor like VSCode or from a Notebook such as Jupyter Notebook, Colab, or Pycharm. The advantage of the latter is that they allow us to work with rich text and view outputs in parts of our code, giving us great flexibility.

# Comments
It is good practice to comment our code, which means adding non-executable text that explains what our code is doing. This will make it easier for us to correct the code later on and for others who want to understand what we are doing. To comment the code, we use the # symbol, which makes any text after it not executed.

```Python
#This is a comment
```
# Variables and object types

We will say that a variable is a "container of information" in which we can "store" different [[objects]]. Variables are generally written in lowercase, without spaces, accents, commas, periods, question marks, or any other character except the underscore. In Python, it is not necessary to explicitly declare the type of object that a variable or collection contains.

To declare a variable, we use:

```Python
variable_name = "Variable Value"
```

The objects we store in variables can be of different types, and depending on the type of object, we change the way we store it.

```Python
integer_object = 2
string_object = "Hello World"
float_object = 2.5
bool_object = False
```

It may happen that we need to convert an object from one type to another. For this, we use type casting, which involves using one of the following [[function]]s, as appropriate."

```Python
int(objeto_float)
float(objeto_int)
str(objeto_int)
bool(objeto_bool)
```
# Arithmetic Operators

Python includes several arithmetic operators used for mathematical operations on numbers. The arithmetic operators include:

- `+`: add two numbers
- `-`: subtracts two numbers
- `*`: multiplies two numbers
- `/`: divides two numbers (returns a floating-point number)
- `//`: divides two numbers (returns the integer part of the division)
- `%`: returns the remainder of the division between two numbers
- `**`: raises a number to a power

Below are some examples:

```Python
a = 10
b = 5

sum_result = a + b
subtraction_result = a - b
multiplication_result = a * b
division_result = a / b
integer_division_result = a // b
remainder_result = a % b
power_result = a ** 2

a = 10
b = 5

c = a + b
d = a * b

print(c) # Output: 15
print(d) # Output: 50

```

Furthermore, Python follows conventional rules for the precedence of arithmetic operators. This means that operations within parentheses are evaluated first, followed by exponentiation, multiplication and division, and finally addition and subtraction. We can use parentheses to force a different order of evaluation.

# Logical and Comparison Operators

In Python, there are three logical operators used to combine logical expressions and produce a true or false result:

- `and`: This operator returns true if both operands are true. Otherwise, it returns false.
- `or`: This operator returns true if at least one of the operands is true. If both operands are false, it returns false.
- `not`: This operator returns the opposite value of the expression's result. If the expression is true, it returns false, and if the expression is false, it returns true.

In addition, comparison operators can be used to create logical expressions. The comparison operators are as follows:

- `==`: This operator returns true if the operands are equal.
- `!=`: This operator returns true if the operands are not equal.
- `>`: This operator returns true if the left operand is greater than the right operand.
- `<`: This operator returns true if the left operand is less than the right operand.
- `>=`: This operator returns true if the left operand is greater than or equal to the right operand.
- `<=`: This operator returns true if the left operand is less than or equal to the right operand.

# Formatting Options

Formatting options in Python refer to the different ways strings can be formatted to include variable values and other elements. The goal of formatting options is to produce strings that are easy to read and understand for end users.

Python offers several formatting options for strings, including:

1. f-strings: f-strings or format strings allow you to include variable values within a string by placing the variable names inside curly braces { }.

```Python
name = "Juan"
age = 25
print(f"Hello, my name is {name} and I am {age} years old")
# Output: Hello, my name is Juan and I am 25 years old
```

2. `str.format()` method: The `str.format()` method allows you to specify variable values within a string using curly braces {}.

```Python
name = "Juan"
age = 25
print("Hello, my name is {} and I am {} years old".format(name, age))
# Output: Hello, my name is Juan and I am 25 years old
```

3. Using % formatting operators: This method is similar to the `str.format()` method, but it uses % formatting operators to specify variable values.

   Very important to note that:
   
   - %s - String (or any object when representing numbers as a string)
   - %d - Integers
   - %f - Floating-point numbers
   - %.f - Floating-point numbers with a fixed number of digits to the right of the decimal point.
   - %b - Integers with binary representation (lowercase/uppercase)
   - %x - Integers with hexadecimal representation (lowercase/uppercase)
   - %o - Integers with octal representation (lowercase/uppercase)

```Python
name = "Juan"
age = 25
print("Hello, my name is %s and I am %d years old" % (name, age))
```

# Data Structures

A data structure is an object that can contain multiple values or elements, such as numbers, strings, [[objects]], or other [[data structures]]. [[data structures]] are a fundamental part of the Python language and are used in many situations to store and manipulate data.

The main data structures that we can find are:

- Variables
- Strings
- Sets
- Lists
- Dicts
- Tuples
## Lists

A list in Python is an ordered and mutable data structure of elements separated by commas and enclosed in square brackets [ ]. The elements can be of different data types, such as numbers, strings, booleans, etc. Lists are used to store collections of related elements and can be modified by adding, removing, or modifying elements. Lists can also be used to represent a [[matrix]] and [[vectors]].

Lists have an index that allows us to access each of the elements belonging to the list, meaning the index of a list specifies the position of an element in the list. In Python, the index starts at zero, which means that the first element of the list has an index of 0, the second element has an index of 1, and so on.

To access a specific element of the list, we can use its index within square brackets. For example, to access the second element of a list called my_list, we would use my_list[1].

We can also use negative indices to access elements from the end of the list. For example, my_list[-1] would access the last element of the list.

Here are some examples:

```python
my_list = [1, 2, 3, 4, 5]
print(my_list[0]) # Output: 1
print(my_list[2]) # Output: 3
print(my_list[-1]) # Output: 5
```

We can also modify elements of the list using their index. For example, to change the second element of my_list to 10, we can do the following:

```python
my_list[1] = 10
print(my_list) # Output: [1, 10, 3, 4, 5]
```

Like all data structures, there are methods that allow us to edit lists.

### List Methods

The main methods of the list class in Python include:

- `append()`: adds an element to the end of the list. Example: `my_list.append(6)`
- `insert()`: inserts an element at a specific position in the list. Example: `my_list.insert(2, 7)` (inserts the number 7 at position 2 in the list)
- `remove()`: removes the first element from the list that matches the specified value. Example: `my_list.remove(3)` (removes the number 3 from the list)
- `pop()`: removes the element at the specified position in the list and returns that element. If no position is specified, it removes and returns the last element of the list. Example: `my_list.pop(2)` (removes the element at position 2 of the list and returns that element)
- `clear()`: removes all elements from the list. Example: `my_list.clear()`
- `sort()`: sorts the elements of the list in ascending order. Example: `my_list.sort()`
- `reverse()`: reverses the order of the elements in the list. Example: `my_list.reverse()`

Here is an example that uses some of these methods:

```python
my_list = [1, 2, 3, 4, 5]
my_list.append(6)
my_list.insert(2, 7)
my_list.remove(3)
deleted = my_list.pop(2)
my_list.sort()
my_list.reverse()
print(my_list) # Output: [6, 5, 4, 2, 1]
```

## Tuples

A tuple in Python is an ordered and immutable data structure of elements separated by commas and enclosed in parentheses ( ). The elements can be of different data types, such as numbers, strings, booleans, etc. Tuples are used to store collections of related elements and are similar to lists, but they cannot be modified by adding, removing, or modifying elements after they have been created.

Tuples, like lists, have an index that allows us to access each of the elements belonging to this tuple, meaning the index of a tuple specifies the position of an element in the tuple. In Python, the index starts at zero, which means that the first element of the tuple has an index of 0, the second element has an index of 1, and so on.

To access a specific element of the tuple, we can use its index within parentheses. For example, to access the second element of a tuple called my_tuple, we would use my_tuple[1].

We can also use negative indices to access elements from the end of the tuple. For example, my_tuple[-1] would access the last element of the tuple.

Here are some examples:

```python
my_tuple = (1, 2, 3, 4, 5)
print(my_tuple[0]) # Output: 1
print(my_tuple[2]) # Output: 3
print(my_tuple[-1]) # Output: 5
```

Tuples are useful when we want to store data that should not change, such as coordinates or constants. They are also often used to return multiple values from a [[function]].

Although tuples are immutable, we can concatenate two or more tuples to create a new tuple containing the elements of both tuples:

```python
my_tuple = (1, 2, 3)
another_tuple = (4, 5, 6)
new_tuple = my_tuple + another_tuple
print(new_tuple) # Output: (1, 2, 3, 4, 5, 6)
```

## Sets

A set in Python is an unordered and mutable collection of unique elements separated by commas and enclosed in curly braces { }. The elements can be of different data types, such as numbers, strings, booleans, etc. Sets are used to store collections of related elements and can be modified by adding or removing elements. Sets can also be used to perform common mathematical operations, such as union, intersection, and difference.

To create an empty set, we can use the [[function]] `set()`:

```python
my_set = set()
print(my_set) # Output: set()
```

To create a set with elements, we can do the following:

```python
my_set = {1, 2, 3}
print(my_set) # Output: {1, 2, 3}
```

We can also create a set from a list:

```python
my_list = [1, 2, 3, 3, 4]
my_set = set(my_list)
print(my_set) # Output: {1, 2, 3, 4}
```

### Set Methods

We can add elements to a set using the `add()` method:

```python
my_set = {1, 2, 3}
my_set.add(4)
print(my_set) # Output: {1, 2, 3, 4}
```

We can remove elements from a set using the `remove()` method:

```python
my_set = {1, 2, 3}
my_set.remove(2)
print(my_set) # Output: {1, 3}
```

We can perform common mathematical operations on sets, such as union, intersection, and difference. For example, to obtain the union of two sets, we can use the `union()` method or the `|` operator:

```python
set1 = {1, 2, 3}
set2 = {3, 4, 5}
union = set1.union(set2)
print(union) # Output: {1, 2, 3, 4, 5}

union = set1 | set2
print(union) # Output: {1, 2, 3, 4, 5}
```

To obtain the intersection of two sets, we can use the `intersection()` method or the `&` operator:

```python
set1 = {1, 2, 3}
set2 = {3, 4, 5}
intersection = set1.intersection(set2)
print(intersection) # Output: {3}

intersection = set1 & set2
print(intersection) # Output: {3}
```

To obtain the difference between two sets, we can use the `difference()` method or the `-` operator:

```python
set1 = {1, 2, 3}
set2 = {3, 4, 5}
difference = set1.difference(set2)
print(difference) # Output: {1, 2}

difference = set1 - set2
print(difference) # Output: {1, 2}
```

We can also perform comparison operations on sets, such as checking if one set is a subset of another set. For example, to check if `set1` is a subset of `set2`, we can use the `issubset()` method:

```python
set1 = {1, 2, 3}
set2 = {1, 2, 3, 4, 5}
print(set1.issubset(set2)) # Output: True
```

We can perform other common operations on sets, such as checking if two sets are equal (`==`), checking if an element is in a set (`in`), and getting the length of a set (`len()`).

Sets are useful when we want to store unique data and perform common mathematical operations on them.

## Dicts 

A dictionary in Python is an unordered and mutable collection of key-value pairs separated by commas and enclosed in curly braces { }. Each key in the dictionary must be unique, and the values can be of different data types, such as numbers, strings, booleans, lists, sets, tuples, or even other dictionaries. Dictionaries are used to store collections of related elements and can be modified by adding, removing, or modifying elements.

To create an empty dictionary, we can use the [[function]] `dict()`:

```python
my_dict = dict()
print(my_dict) # Output: {}
```

To create a dictionary with elements, we can do the following:

```python
my_dict = {"name": "Juan", "surname": "Pérez", "age": 30}
print(my_dict) # Output: {'name': 'Juan', 'surname': 'Pérez', 'age': 30}
```

We can also create a dictionary from a list of key-value pairs:

```python
my_list = [("name", "Juan"), ("surname", "Pérez"), ("age", 30)]
my_dict = dict(my_list)
print(my_dict) # Output: {'name': 'Juan', 'surname': 'Pérez', 'age': 30}
```

We can access the values of a dictionary using its keys. For example, to access the value corresponding to the key "name" in a dictionary called `my_dict`, we can do the following:

```python
my_dict = {"name": "Juan", "surname": "Pérez", "age": 30}
print(my_dict["name"]) # Output: Juan
```

We can also use the `get()` method to access the values of a dictionary. The advantage of `get()` is that if the key does not exist in the dictionary, it returns a default value instead of raising an error:

```python
my_dict = {"name": "Juan", "surname": "Pérez", "age": 30}
print(my_dict.get("name", "Default value")) # Output: Juan
print(my_dict.get("address", "Default value")) # Output: Default value
```

We can modify the values of a dictionary using its keys. For example, to change the value corresponding to the key "age" in a dictionary called `my_dict` to 40, we can do the following:

```python
my_dict = {"name": "Juan", "surname": "Pérez", "age": 30}
my_dict["age"] = 40
print(my_dict) # Output: {'name': 'Juan', 'surname': 'Pérez', 'age': 40}
```

If the key does not exist in the dictionary, a new key-value pair is added to the dictionary:

```python
my_dict = {"name": "Juan", "surname": "Pérez", "age": 30}
my_dict["address"] = "Calle 123"
print(my_dict) # Output: {'name': 'Juan', 'surname': 'Pérez', 'age': 30, 'address': 'Calle 123'}
```

We can remove elements from a dictionary using the `del` keyword and the corresponding key:

```python
my_dict = {"name": "Juan", "surname": "Pérez", "age": 30}
del my_dict["age"]
print(my_dict) # Output: {'name': 'Juan',

 'surname': 'Pérez'}
```

Like all classes, dictionaries have methods that allow us to edit them.

### Dictionary Methods

The main methods of the `dict` class in Python include:

- `keys()`: returns a list with the keys of the dictionary. Example: `my_dict.keys()`
- `values()`: returns a list with the values of the dictionary. Example: `my_dict.values()`
- `items()`: returns a list of tuples with the key-value pairs of the dictionary. Example: `my_dict.items()`
- `clear()`: removes all elements from the dictionary. Example: `my_dict.clear()`
- `update()`: updates the dictionary with the key-value pairs from another dictionary or from a list of key-value pairs. Example: `my_dict.update({"address": "Calle 123", "phone": "555-1234"})`

Here's an example that uses some of these methods:

```python
my_dict = {"name": "Juan", "surname": "Pérez", "age": 30}
keys = my_dict.keys()
values = my_dict.values()
items = my_dict.items()
my_dict.update({"address": "Calle 123", "phone": "555-1234"})
print(my_dict) # Output: {'name': 'Juan', 'surname': 'Pérez', 'age': 30, 'address': 'Calle 123', 'phone': '555-1234'}
```
