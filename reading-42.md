# Reading 42

## [Dunder Methods](https://dbader.org/blog/python-dunder-methods)

- the dunder methods are known as the python data model
- __repr__ is the offical string used for dev
- __str__ is the unoffical string for users
- There are a lot of dunder methods to implement that make working in OOP much cleaner

## [Iterators](https://dbader.org/blog/python-iterators)

- objects with __iter__ or __next__ methods work with for loops
To iterate over an object the object itself must have the __iter__ class that references a return from a help class that the __iter__ class passes source information to. This helper class will containt the __next__ method and is responsible for the returning value.

Iterating an over an object this way if very memory efficent. It also is very powerful, because it allows the programmer to output something indefinatly. This could not be done with a list because list cannot be infitely long. This can also be done with the build int init() and next() methods.

To shorted the code into one class have both the __iter__ and __next__ methods in the same class. The __iter__ method should return self while the __next__ method should return self.value.

It is possible to control how many times the iteration occurs. In the __next__ method set up a conditional that will raise a StopIteration error if the amount of iterations desired have been run. To reset the iteration you must instantiate another __iter__ of the instance.

For this to work in both python 3 and 2 create a next method without the dunder and reference and return the __next__ method. Python 2's next is equivalant to python 3's __next__.

## [Generators](https://dbader.org/blog/python-generators)

Generators make write iterators easier.

To write a generator write it as a normal function that takes in a value. Then create a while loop that instead of using return uses yield to "return" the value from the for loop.
yeild allows for temporary caller passback and stores local variables temporarily.

A boundary function can be set up to control the number of iterations using a number of iterations argument and a for loop yielding the values.

## Bookmarks

- [What are Generators](https://realpython.com/lessons/what-are-python-generators/)
- [Decorators](https://realpython.com/primer-on-python-decorators/)
