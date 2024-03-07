### *Explain the concept of variable scope in Python and describe the difference between local and global scope. Provide an example illustrating the usage of both* ###

- In Python, the concept of variable scope determines the part of a program where a variable is accessible. Scope essentially defines the visibility of a variable within different areas of the code. Python utilizes the LEGB rule to resolve variable names, which stands for Local, Enclosing, Global, and Built-in scopes,

- Local scope refers to variables defined within a function. These variables are only accessible within the function they are defined in and cease to exist once the function execution is completed. They are not accessible from outside the function.

- Global scope refers to variables defined at the top level of a script or module or explicitly declared global using the global keyword within a function. These variables are accessible throughout the file, and also inside any function, provided they are declared as global within those functions if they intend to modify them.



### *How do the global and nonlocal keywords work in Python, and in what situations might you use them?* ###

- The global and nonlocal keywords in Python are used to modify the scope of variables outside of the current scope. They allow you to assign values to variables that exist in the global scope or in an enclosing scope

- The global keyword is used to declare that a variable inside a function is global. This means that any changes made to this variable inside the function will reflect in the global scope of the variable. It is particularly useful when you need to change or update a global variable from within a function.

```python
x = 7

def modify_global():
    global x  # Declaring x as global
    x = 10    # Modifying the global x, not a local variable

modify_global()
print(x)  # This will print 10, showing that the global x has been changed
```

- The nonlocal keyword is used within nested functions to declare that a variable refers to a previously bound variable in the closest enclosing scope (excluding globals). This is useful when you want to modify a variable in an enclosing scope that is not the global scope.

```python
def outside():
    x = "local"

    def inside():
        nonlocal x  # Declare x as nonlocal
        x = "nonlocal"  # This modifies the x defined in the outside function

    inside()
    print(x)  # This will print "nonlocal", showing that the inside function modified the outside x

outside()
```


### *In your own words, describe the purpose and importance of Big O notation in the context of algorithm analysis* ###

- Big O notation serves as a fundamental tool in the field of computer science for understanding, comparing, and optimizing algorithms based on their theoretical performance and scalability. It can help developers and computer scientists make informed decisions about which algorithms to use or how to design algorithms for specific problems, particularly when dealing with large datasets or systems where performance and efficiency are critical.

### *Based on the Rolling Dice Example, explain how you would simulate a dice roll using Python. Describe how you would use code to calculate the probability of rolling a specific number (e.g., the probability of rolling a 6) over a large number of trials* ###

```python
import random

# Definition of the roll_dice function
def roll_dice():
    return random.randint(1, 6)

"""Function to simulate dice rolls and calculate the probability of rolling a specific target number and taking two arguments trails which is the number of dice should be rolled and target the number whose rolling probability we want to calculate """
def simulate_dice_rolls(trials, target):
    count = 0
    for _ in range(trials):
        if roll_dice() == target:
            count += 1
    return count / trials

# rolling a dice 100,000 times and calculating the probability of rolling a 6
trials = 100000
target_number = 6
probability = simulate_dice_rolls(trials, target_number)
print(f"The probability of rolling a {target_number} is approximately {probability}")
```


[Reference](https://realpython.com/python-scope-legb-rule/)

[Reference](https://www.youtube.com/watch?v=dNorFNlDbX0)

[Reference](https://web.archive.org/web/20220608035657/https://artofproblemsolving.com/wiki/index.php/Basic_Programming_With_Python#Random)

