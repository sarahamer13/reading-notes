### *What does .map() return?* ###

- It returns an array that will have the same length as the original array

### *If I want to loop through an array and display each value in JSX, how do I do that in React?* ###

- By using .map() to loop through an array and display each value

### *Each list item needs a unique ____* ###

- Key

### *What is the purpose of a key?* ###

- To give each object a unique key

### *What is the spread operator?* ###

- The spread operator is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.

### *List 4 things that the spread operator can do* ###

- Using Math functions
- Using an array as arguments
- Adding an item to a list
- Adding to state in React


### *Give an example of using the spread operator to combine two arrays* ###
 
- const myArray = [Hi,there,!] const yourArray = [I,am,here`] const ourArray = […myArray,…yourArray] console.log(…ourArray) // ‘Hi’ ‘there’ ‘!’ ‘I’ ‘am’ ‘here’

### *Give an example of using the spread operator to add a new item to an array* ###

const fruits = ['🍏','🍊','🍌','🍉','🍍']
const moreFruits = [...fruits];
console.log(moreFruits) // Array(5) [ "🍏", "🍊", "🍌", "🍉", "🍍" ]
fruits[0] = '🍑'
console.log(...[...fruits,'...',...moreFruits]) //  🍑 🍊 🍌 🍉 🍍 ... 🍏 🍊 🍌 🍉 🍍

### *Give an example of using the spread operator to combine two objects into one* ###

- const ObjectOne = {name: Sarah};
- const ObjectTwo = {state: California};
- const ObjectThree = {...ObjectOne, ...ObjectTwo}
Result will be: ObjectThree {name:Sarah, state: California}



### *In the video, what is the first step that the developer does to pass functions between components?* ###

- creating the function

### *In your own words, what does the increment function do?* ###

- It takes in the person, then increases the count depending on which name is passed through

### *How can you pass a method from a parent component into a child component?* ###

- By using this."the name of the method" 


(References:
https://legacy.reactjs.org/docs/lists-and-keys.html
https://medium.com/coding-at-dawn/
how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab
https://www.youtube.com/watch?v=c05OL7XbwXU )

