
### *Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?* ###

- Based on the diagram, it looks like componentDidMount happens before the render occurs.


### *What is the very first thing to happen in the lifecycle of React?* ###

- When an instance of a component is being created and inserted into the DOM it occurs during the mounting phase. Constructor, static getDerivedStateFromProps, render, componentDidMount, and UNSAFE_componentWillMount all occur in this order during mounting.

### *Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates* ###

- Constructor 
- React Updates
- Render
- ComponentDidMount
- ComponentWillUnmount

### *What does componentDidMount do?* ###

- This method is invoked immediately after a component is mounted. If you need to load anything using a network request or initialize the DOM, it should go here. This method is a good place to set up any subscriptions. If you do that, don’t forget to unsubscribe in componentWillUnmount().

setState() can be called here, but it should be used sparingly, because it will cause a rerender, which can lead to performance issues.

### *What types of things can you pass in the props?* ###

- Props are for things that you would pass into a function, what you want to initialize your component to or to what you want your component to render.

### *What is the big difference between props and state?* ###

- State is handled inside the component, while props you pass into a component and it's handled outside the component.

### *When do we re-render our application?* ###

- It will re-render your application when you change the state inside your component

### *What are some examples of things that we could store in state?* ###

- A form would be stored in state. Also, If you want the description or title to change based on user input, you would store it in state as well.


(Reference: https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093

https://www.youtube.com/watch?v=IYvD9oBCuJI)

## Things I want to know more about 

- Learning more about props
