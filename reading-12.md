# Reading 12

## [Pandas in 10](https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html)

- import: import numpy as np, import pandas as pd
- `s = pd.Series([1, 3, 5, np.nan, 6, 8])` - object list
- `dates = pd.date_range("20130101", periods=6)` - date array
- `df2 = pd.DataFrame(object)` - data frame based on object
- `df.head()` - top of data
- `df.tail(3)` - end of data
- numpy arrays have one data type and panda can have many
- `df.to_numpy()` - to convert
- `df.describe()` - statistic summary
- slice and get data like a list
- both endpoints are included in a slice
- can select by position
- can do operational selection
- use `isin()` to filer
- can set data by label, position or by setting a numpy array
- `np.nan` means empty data
- `.fillnan()` to fill missing data
- `isna()` to get boolean representation of present data
- `.mean()` to get mean on one axis at a time
- `.apply(function)` to apply function to data
- str.lower() makes everything lower case
- `concat()` to merge data
- `.groupby()` to group and then you can chain other actions
- `stack()` will compress that data, it's inverse is `unstack()`
- `pivot_table()` for table
- `.plot()` to plot a graph
- can plot multiple graphs on one

## [What is Pandas](https://www.youtube.com/watch?v=dcqPhpY7tWk&t=391s)

- can read exel sheets
- other functions that read other file types
- .drop() will get rid of columns that you don't want
- allows for different types of data visualization
- .index tell you how the data has been loaded in

## [Bookmark]

- [Pandas - Getting Started](https://pandas.pydata.org/pandas-docs/stable/getting_started/intro_tutorials/index.html)
- [Real Python - Pandas Tutorials](https://realpython.com/learning-paths/pandas-data-science/)
- [Master Pandas](https://towardsdatascience.com/be-a-more-efficient-data-scientist-today-master-pandas-with-this-guide-ea362d27386?gi=ab35966f4cf2)
