# Reading 19

## [Python Regular Expressions Tutorial](https://www.datacamp.com/community/tutorials/python-regular-expression-tutorial)

- useful functions:
  - compile(), search(), findall(), sub()

```python
import re
pattern = r"Cookie"
re.match(pattern, string)
re.search(pattern, string).group() # search() scans through the string to find the first match and group returns the string matched by the re. 

```

- .match() returns match object or none
- r is raw string literal
- ^ matches start
- $ matches end
- [abc] matches a, b or c
- if an escape character is proceded by a \ then it will be escaped otherwize \ is like any other char
- \w lowercase w
- \W uppercase W
- \s matches a single white space 
- \S matches any character not part of the \s
- \d matches decimal digit
- \D matches any character not decimal digit
- \t matches tab
- \n matches new line
- \r matches return
- \A matches only at the start of the String. works accross multiple lines
- \Z matches only at the end of the string
- + checks if the preceding char appears one or more times
- * checks if the preceding char appears zero or more times
- ? checks if the preceding char appears exactly zero or one time
- {x} repead exactly x number of times
- {x,} repeat at least x times or more
- {x, y} repeat at least x time but no more than y times
- mathc.group() will get you the whole string
- match.group(1) will get you the first group and so on
- can name groups
- greedy qualifiers will gety you more of the surrounding string
- re.complie(pattern, flags = 0) save the patters for reuse as object
- search(pattern, string, flags = 0) retuns the first pattern match and none otherwize
- match(pattern, string, flags = 0) retuns a corresponding match object if zero or more character in the beginning of string match the pattern else it returns none
- findall(pattern, string, flags = 0) finds all the possible matches in the entire sequence and returns them as a list of strings.
- finditer(string, [position, end_position]) finds all the possible matches in the entire sequence but returns regex match objects as an iterator
- sub(pattern, repl, string, count=0, flags=0) the substiture function. returns the string obatained by subsitution
- subn() similar to sub(), but returns a tuple containing the new string value and the number of replacments that we performed
- split(string, [maxsplit = 0]) splis the string wherever the pattern matches and retuns a list
- start() returns the starting index of the match
- end() retuns the index where the match ends
- span() returns a tuple containing the (start, end) position of match
- IGNORECASE(I) allos for insensivitve matching
- DOTALL(S) allows . to match to any character including a new line
- MULTILINE(M) allows the start of string and end anchor to match newlines as well
- VERBOSE(X) allows you to write white space and comment iwhtin a regular expression to make it more readable

## [shutil](https://pymotw.com/3/shutil/)

- copyfile() copies contents of the source to destination and raises IOError if it doesn't have the permission to write to the file
- copy() interprets the name of the command line file
- copy2() is like copy() but includes the access and modificiation times in the metadata copied to the new file
- to compy permissions from one file to another use copymode()
- copystat() is used to copy other metadata about the file
- copytree() will copy the directory tree
- rmtree() will remove a directory and its contents
- move() moves a file or directory from one place to another
- which() scans a search ptath looking for a named file
- make_archive() will make a new archive file
- disk_usage() retuns a tuple with the total space, the amount being used, adn the amount remaining

## Bookmarks

- [Automation Ideas](https://www.youtube.com/watch?v=qbW6FRbaSl0&t=69s)
- [Automating Your Browser and Desktop Apps](https://www.youtube.com/watch?v=dZLyfbSQPXI)
- [Watchdog](https://pythonhosted.org/watchdog/)
