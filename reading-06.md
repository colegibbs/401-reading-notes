# Reading 06: Ten Thousand Game 1

## [How to use Random Module](https://www.pythonforbeginners.com/random/how-to-use-the-random-module-in-python)

- Allows you to generate random numbers
- Use when you need something to be picked randomly
- functions:
  - .randint(start, finish)
  - .random
  - .choice(list) - picks randomly from list
  - .shuffle(list) - randomizes list order
  - .randrange(start, end, step) - random input from range with step

## [What is Risk Analysis](https://www.edureka.co/blog/risk-analysis-in-software-testing/)

- risk - unexpected behavior in code
- risk analysis - identifying the risk
- possible risks:
  - Use of new hardware
  - Use of new technology
  - Use of new automation tool
  - The sequence of code
  - Availability of test resources for the application
- risks are considered high, medium, or low
- risk identification
  - Buisness risk - risk coming from company or customer
  - Testing risk - know the testing tools and software well
  - Premature Release risk - unsatisfactory or untested software
  - Software rist - process
- asses risks by: Effect, cause and likelyhood
- How: 
  - Searching the risk
  - analyze the impact of each risk
  - measures for the risk identified

## [Test Coverage](https://martinfowler.com/bliki/TestCoverage.html)

- helps find untested code
- testing must be quality
- 80 to 90 coverage is good
- tested well when:
  - "You rarely get bugs that escape into production"
  - "You are rarely hesitant to change some code for fear it will cause production bugs"
- if tests slow you down then you may have too many tests

## [Big O notation](https://www.youtube.com/watch?v=v4cd1O4zkGw)

- transfering data over internet takes more time the more info there is
- O(1) - constant time w/ input
- O(n) - scales w/ input
- O(n^2) - nested
- four important rules:
  - if you hade two different steps, add the steps
  - drop constants
  - different in puts mean different variables
  - drop non-dominate terms

## Bookmark

- [Python Random](https://docs.python.org/3/library/random.html)
- [What is Dependency Injection](https://www.freecodecamp.org/news/a-quick-intro-to-dependency-injection-what-it-is-and-when-to-use-it-7578c84fa88f/)
