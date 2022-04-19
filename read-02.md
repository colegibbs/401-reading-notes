# Reading 02: Testing and Modules

## [Reading: In Tests We Trust - TDD with Python](https://code.likeagirl.io/in-tests-we-trust-tdd-with-python-af69f47e6932?gi=e8085abb1f9c)

- unit tests is code that tests your codes functionality based on input and output
- Test Driven Development - write tests first
- Tests use your code to evaluate expected outputs based on inputs
- test name needs to be descriptive
- test file should reflect the name of the file it is testing on
- AAA - Arrange, Act, Assert
- Steps: write a failing test, write the feature and make the test pass, refractor the code
- makes you consider design
- Code will be more reliable this way

## [Reading: If name equals main](https://www.geeksforgeeks.org/what-does-the-if-__name__-__main__-do/)

"Every Python module has it’s __name__ defined and if this is ‘__main__’, it implies that the module is being run standalone by the user and we can do corresponding appropriate actions.
If you import this script as a module in another script, the __name__ is set to the name of the script/module.
Python files can act as either reusable modules, or as standalone programs.
if __name__ == “main”: is used to execute some code only if the file was run directly, and not imported."

## [Video: What on Earth is Recursion](https://www.youtube.com/watch?v=Mv9NEXX1VHc)

- using functions to define themselves
- using equations to define themselves
- argument value will constantly, predictably change
- the base argument allows the function to go all the way down the chain of values and once it hits the base it calculates all the way back up

## Bookmarks

- [Google for Education: Python Lists](https://developers.google.com/edu/python/lists)
- [Google for Education: Python Strings](https://developers.google.com/edu/python/strings)
- [Python Modules and Packages](https://realpython.com/python-modules-packages/)
- [Pytest Documentation](https://docs.pytest.org/en/latest/)
- [PyTest Tutorial](https://www.guru99.com/pytest-tutorial.html)
