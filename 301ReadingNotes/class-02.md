# State and Props

# React lifecycle

### 1-Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?

A- Render.

### 2-What is the very first thing to happen in the lifecycle of React?

A- getDerivedStateFromProps() is the first method to be called and the very first thing in the life cycle of react.

### 3-Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates

A- Constructer => Render => React Updates => ComponentDidMount => componentWillUnmount.

### 4-What does componentDidMount do?

A- This method is invoked right after the component has been mounted so its used to load anything using a network request or initialize the DOM.


# React State Vs Props

### What types of things can you pass in the props?

A- Props are like arguments of a function, which means we can pass pretty much any data type such as Int, Strings and Arrays.

### What is the big difference between props and state?

A- State is handled in the component and it can be updated inside the component while props are handled outside of the component and must be updated outside of the component.

### When do we re-render our application?

A- When the component is not static and needs to be updated after the user has interacted with it, such as a counter component.

### What are some examples of things that we could store in state?

A-Inside of a form where we can use state to store the form information to what the user updates or adds.



## Things I want to know more about

-Instead of using classes, in state and lifecycle of react documentation, I see that they are used as function not a class.

-I am curious to furthermore learn/make interactable components such as small games.







[Go Back](https://musaabshalaldeh.github.io/reading-notes/)