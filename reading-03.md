
# Reading 03: FileIO & Exceptions

## [Reading: Read & Write Files in Python](https://realpython.com/read-write-files-python/)

- a file is a stored bytes
- file comp:
  - "Header: metadata about the contents of the file (file name, size, type, and so on)
  - Data: contents of the file as written by the creator or editor
  - End of file (EOF): special character that indicates the end of the file"\
- extension determines type
- file path: where the file exists
- need to account for file operating system origin
- must read the file with the same character encoding is was made with
- to open file: open("file_path.ext)
- close the file when you are done with it
- close: variable_name.close() or with statement
- with staments are bests
  - put filepath and mode in with statment arguments
- file obj:
  - text files
  - buffered Binary files
  - raw binary files
- text files
  - read(bytes)
  - readline(bytes)
  - readlines
- change files:
  - write()
- can work with multiple files open
- to use with statments in a class you must use a context manager
- There are usful bulit in libaraies

## [Reading: Exceptions in Python](https://realpython.com/python-exceptions/)

- sytax error or exeption
- syntax error: parser found an incorrect statement
- exeption: syntactically correct code as an error
  - will tell you wheat type of expetion error
- can throw your own exeption inside of in if statment with `raise("error message")
- assert allows for a condition and error message
  - `assert (condition), "error message"
- in a try, except if there is an error in the try the exept will run based on the exception type
- can add else to the end of a try, except to add code that runs if the except did not run
- finally will run no matter what at the end of a try, exept

## Bookmark

- [Read & Write Files in Python - Companion Video](https://realpython.com/courses/reading-and-writing-files-python/)
- [Reading and Writing Files in Python Quiz](https://realpython.com/quizzes/read-write-files-python/)
