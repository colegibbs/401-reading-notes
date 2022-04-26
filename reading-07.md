# Reading 07: Ten Thousand 2

## [Python Scope](https://realpython.com/python-scope-legb-rule/)

- globals() will give you a dictonary of all the global variables in the file
- search for names with globals() using if statements
- locals() returns all of the local functions and variable names
- if you call locals() in the global scope: globals() == locals()
- chaning a value in locals() does not change the variable name
- vars() returns a dictionary in all values in side of dictionary
- it calls the `__dict__` of the dictionay
- at the global level `vars() == locals()
- dir() w/ no arguments will return names at the global scope

## [Don’t be CONFUSED by BIG O notation anymore!](https://www.youtube.com/watch?v=5Uqawfl0VHQ)

- way of comparing algorithms and how they perform
- worst case senario
- O(1) - constant
- O(log n) - logarithmic running
- O(n) - Linear Running
- O(n log n) - Log-linear running
- O(n^k) - Polynomial Running time
- O(C^n) - exponential running
- time graph: x: Number of Inputs, y: Time
- as binary search runs it scales log
- The different between the complexities can be huge
- images can be sorted through in all differnt ways
