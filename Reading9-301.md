
### *What is functional programming?* ###

- Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data

### *What is a pure function and how do we know if something is a pure function?* ###

- It returns the same result if given the same arguments (it is also referred as deterministic)

- It does not cause any observable side effects

### *What are the benefits of a pure function?* ###

- The code’s definitely easier to test. We don’t need to mock anything. So we can unit test pure functions with different contexts:

- Given a parameter A → expect the function to return value B
- Given a parameter C → expect the function to return value D

### *What is immutability?* ###

- When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.

### *What is Referential transparency?* ###

- Basically, if a function consistently yields the same result for the same input, it is referentially transparent

### *What is a module?* ###

- It's essentially a JavaScript file that has reusable codes throughout node.js application

### *What does the word ‘require’ do?* ###

- It allows information that is stored in one module to be used in another module

### *How do we bring another module into the file the we are working in?* ###

- We have to export the function and import them in the file we want to call the functions.

### *What do we have to do to make a module available?* ###

- Export it in the module where it was declared.

(Reference: https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa, https://www.youtube.com/watch?v=xHLd36QoS4k)

