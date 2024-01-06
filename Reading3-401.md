### *What is the purpose of the ‘with’ statement when opening a file in Python, and how does it help manage resources while reading and writing files?* ##

- The with statement automatically takes care of closing the file once it leaves the with block, even in cases of error. It allows for cleaner code and makes handling any unexpected errors easier for you.

### *Explain the difference between the ‘read()’ and ‘readline()’ methods for file objects in Python. Provide examples of when to use each method* ###

- read(): This method is used to read the entire content of the file as a single string. Use read() when you want to read the entire content of the file as a single string.

```python
with open('music_genres.txt', 'r') as reader:
    # Read & print the entire file
    print(reader.read())
Pop
Rock
Hip Hop
Jazz
Country
Electronic
Classical
R&B
Reggae
Folk
```

- readline(): This reads the remaining lines from the file object and returns them as a list. Use readline() when you want to read the file line by line, or when you only need a specific line from the file.

```python
with open('music_genres.txt', 'r') as reader:
    # Read & print the first 5 characters of the line 5 times
    print(reader.readline(5))
    print(reader.readline(5))
    print(reader.readline(5))
    print(reader.readline(5))
    print(reader.readline(5))

Pop
Rock
Hip H
op
Jazz
```

### *Briefly describe the concept of exception handling in Python. How can the ‘try’, ‘except’, and ‘finally’ blocks be used to handle exceptions and ensure proper execution of code? Provide a simple example* ###

- A Python program terminates as soon as it encounters an error.In Python, an error can be a syntax error or an exception.

- The try and except block in Python is used to catch and handle exceptions. Python executes code following the try statement as a “normal” part of the program. The code that follows the except statement is the program’s response to any exceptions in the preceding try clause.

- Finally enables you to execute sections of code that should always run, with or without any previously encountered exceptions.

```python
try:
    # Attempt to open and read a file
    with open('nonexistent_file.txt', 'r') as file:
        content = file.read()
        print("File content:", content)

except FileNotFoundError:
    print("Error: File not found!")

finally:
    print("Cleanup: This block ensures resource cleanup or final actions.")

```
[Reference1](https://realpython.com/read-write-files-python/)

[Reference2](https://realpython.com/python-exceptions/)
