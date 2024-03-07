### *What is the basic syntax of Python list comprehension, and how does it differ from using a for loop to create a list? Provide an example of a list comprehension that squares the elements in a given list of integers* ###

- The basic syntax for a Python list comprehension is [expression for item in iterable_object], where expression represents the operation performed on each item in the iterable_object, creating a new list. This syntax differs from using a for loop to create a list by being more concise and often more readable, requiring less code for the same operation. For example, to square the elements in a given list of integers using list comprehension,  we would write: squared_list = [item**2 for item in original_list], where original_list is a list of integers​​.

### *What is a decorator in Python?* ###

- In Python, a decorator is a function that allows you to wrap another function in order to extend its behavior without permanently modifying it. Decorators take a function as an argument, add some functionality to it, and return a new function. They are identified by the @ symbol above the function definition. This feature provides a flexible way to add or modify the behavior of functions or methods, making code cleaner and more Pythonic



### *Explain the concept of decorators in Python. How do they work, and what are some common use cases for them? Provide an example of a simple decorator function from the reading* ###

- Decorators in Python are a powerful tool that allows for the modification of functions or methods in a reusable and concise way. They work by taking a function, adding some functionality to it, and returning a modified function. Common use cases include logging, caching, access control, and performance measurement. A simple example of a decorator involves wrapping a function with additional code that executes before and after the target function, effectively extending its behavior without modifying its core logic

```python
def decorator(func):
    def wrapper():
        print("Something is happening before the function is called.")
        func()
        print("Something is happening after the function is called.")
    return wrapper

@decorator
def show_message():
    print("The function is now running.")


show_message()
```
The result will be :

- Something is happening before the function is called.
- The function is now running.
- Something is happening after the function is called.

[Reference](https://www.pythonforbeginners.com/basics/list-comprehensions-in-python)

[Reference](https://realpython.com/primer-on-python-decorators/)


