# Reading 9: Ten Thousand 4

## [Dunder Methods](https://dbader.org/blog/python-dunder-methods)

- allows you to emulate the behavior of built in language features
- `__init__` sets up the class
- common practice to provide string represintation
  - `__str__` for informal string
  - `__repr__` for formal string
-  `__len__` and `__getitem__` are also dunder methods
- `__reversed__`
- `__eq__` for equivalients
- `__lt__` for greater or less than
- `__add__`
- `__call__` allows you to call the class like its a function and specified behavior will execute
- `__enter__` and `__exit__` allows you to use the class in a with statement and the methods will execute on the enter and exit of the with statement respectively

## [Statistics - Probability](https://www.dataquest.io/blog/basic-statistics-in-python-probability/)

- probability - the chances of something happening
- sample space - the possible events that can happen
- probability = number of times event occurs / sample space
- statistics is probability calculated from data in the real world
- the more trials, the less error margin
- normal distribution - graph looking like a single hill, symmetrical
- high point reperesents the mean
- when comparing two normal distributions if the means are closer they are more likely to be similar and if the means are farther they are more likely to be different
- Central Limit Theorm
  - says that if you do many trials, the distribution will look like the normal districution
- Three sigma rule
  - given normal distribution
    - 68% of observations will fall between one standard deviation of the mean
    - 95% will fall within tow
    - 99.7% will fall within three
  - any values three standard deviations from the mean should be treated with caution and are called the rarity of extream values
- Z-score
  - answers "given a data point, how far away is it from the mean?"
  - z-score = (data point - mean) / the standard deviation
- Z-table is the is the cumulative probability that a certain z-score occured

## [Intro to Statistics](https://www.youtube.com/watch?v=MdHtK7CWpCQ)

- collection of princiles and procedure to gain info to make decisions
- identifying risk factor
- concept 1: statistical features
  - most used
  - bias, variant, mean , median, percentials
  - box plot: displaying data based on a few statistical features
  - account for outliers
  - short = data is similat
  - tall = data is different
  - median near bottom = data has lower values
  - median near bottom = data has higher values
  - median not near middle = squed data
- probability distribution
  - range of 0 to 1
  - is a function
  - many times of different distributions
  - uniform - only occursr in a range
  - normal - defined by mean and standard deviation
  - poisson - like normal, but accounts for schequed data
  - power law = functional realtionship between quanitities - if one changes, then the other changes
- Bayesian statistics
  - frequency - parameters fixed, data varies, probability, no prior
  - there is a bayes theorem
  - bayes theorem simplifies a lot of complex concepts
  - can predict disease probability

## [Intro to Statistics](https://www.youtube.com/watch?v=MdHtK7CWpCQ)

- the guy in the last video scammed people
- 