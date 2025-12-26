#Python

[[Python]] is a multi-paradigm programming language, which means it supports different programming approach one of them are Object-Orientend Programming, this type of programming are different of Procedure-Oriented Programming in which usually we start programming (instructions are then organized into functions. The program is divided into a collection of variables, data structures, and routines to accomplish different tasks.)

The object-oriented programming breaks the programming task into **objects**, which combine data (known as attributes) and behaviors/functions (known as methods). Therefore, there are two main components of the OOP: **class** and **object**.

## Class and object

Before explain class and object we will expose a example of the notation to have a idea about we're talking

```
class User():
	name = "Juan"
	surname = "Dueñas"

usuario = User

usuario.name()
>>> Juan
usuario.surname()
>>> Dueñas

```

A class is a schema used to define a logical grouping of data and functions. To create a class we should use the word `class` and then put the first letter of the name in uppercase, before specify the methods of the class. In the example the **class is User** and the **methods of that class are name and surname**.

## init method

The **__init__** is one of the special methods in Python classes that is run as soon as an object of a class is instantiated (created). It assigns initial values to the object before it is ready to be used. Note the two underscores at the beginning and end of the `init`, indicating this is a special method reserved for special use in the language. In this `init`method, you can assign attributes directly when you create the object.

The particular argument `self` refers to the object itself; conventionally, we use `self` to name it. Through this self parameter, instance methods can freely access attributes and other methods in the same object. When we define or call an instance method within a class, we need to use this self parameter.

These attributes can be accessed by all the other methods defined in the class with `self.attribute`

![[Pasted image 20240612181748.png]]

We can also modify the atributes of the classes outside the class just by accessing to the atribute we want to modify.

``` 
class Student():

    def __init__(self, sid, name, gender):

        self.sid = sid
        self.name = name
        self.gender = gender
        self.type = 'learning'

    def say_name(self):

        print("My name is " + self.name)

usuario = Student(sid = "214", name = "Juan", gender = "M")
usuario.say_name()

>>> My name is Juan

usuario.name = "David"
usuario.say_name()

>>> My name is David
```

We can delete instances atributes following `del NameClass.atribute`, also delete objects  with `del NameClass
# Class Atributes

There are another type of attributes called class attributes, which will be shared with all the instances created from this class. In defining a class attribute, we must define it outside of all the other methods **without** using `self`. To use the class attributes, we use `ClassName.attribute`, which in this case is `Student.n`. This attribute will be shared with all the instances that are created from this class.

```
class Student():

    n_instances = 0

    def __init__(self, sid, name, gender):

        self.sid = sid
        self.name = name
        self.gender = gender
        self.type = 'learning'
        Student.n_instances += 1

    def say_name(self):

        print("My name is " + self.name)

    def report(self, score):

        self.say_name()
        print("My id is: " + self.sid)
        print("My score is: " + str(score))

    def num_instances(self):

        print(f'We have {Student.n_instances}-instance in total')
```


# Bibliography

- Udemy - Python sin fronteras, HTML, CSS, Flask y MySQL
- Book Python Programming and Numerical Methods, A Guide for Engineers and Scientists https://pythonnumericalmethods.studentorg.berkeley.edu/
