# Reading 08: Ten Thousand 3

## [List Comprehensions](https://www.pythonforbeginners.com/basics/list-comprehensions-in-python)

- comprehenision features keep your code readable and elegant
- syntax: `my_new_list = [ expression for item in list ]`
- faster than most other methods
- `digits = [x for x in range(10)]` - list from 0 to 9
- for every x in range, inflict the expression
- filter:
  - `even_numbers = [ x for x in range(1,20) if x % 2 == 0]`
  - if statement after list
- can also be used on strings
- list comprehension always return a list
- `nums = [x+y for x in [1,2,3] for y in [10,20,30]]` - allows for additon of all numbers with eachother

## Bookmark
- [Debugging with PySnooper](https://www.pythonpodcast.com/pysnooper-python-debugging-episode-241/)
- [Primer on Decorators](https://realpython.com/primer-on-python-decorators/)
