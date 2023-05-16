### *What is a ‘call’?* ###

- invoking a function

### *How many ‘calls’ can happen at once?* ###

- It happens one at a time

### *What does LIFO mean?* ###

- Last In, First Out. It's used to temporarily store and manage function invocation (call)

### *What causes a Stack Overflow?* ###

- A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accommodate before throwing a stack error

### *What is a ‘reference error’?* ###

- When you try to use a variable that is not yet declared.

### *What is a ‘syntax error’?* ###

- This occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.

### *What is a ‘range error’?* ###

- When you try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.

### *What is a ‘type error’?* ###

- This types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.

### *What is a breakpoint?* ###

- A breakpoint is a point in the code where execution is temporarily paused, allowing the developer to inspect the state of the application and debug it.

### *What does the word ‘debugger’ do in your code?* ###

- It adds a breakpoint to the code, which allow the developer to review the things that are happening to that particular point

(References: https://medium.freecodecamp.org/understanding-the-javascript-call-stack-861e41ae61d4 ,
https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c
)