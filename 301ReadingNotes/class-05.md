# Putting it all together


### How would you break a mock into a component heirarchy?

A-By breaking down the componenet into different parts and having each element related to a parent element, as in what is related to cloths is under cloths tab and whats related to plastic products is under plastic products tab.

### What is the single responsibility principle and how does it apply to components?

A-Single responsibility principle is that a component should ideally only do one thing and if it expands on doing more than 1 thing it should be broken down into multiple components.

### What does it mean to build a ‘static’ version of your application?

A-To build a version of your app that takes your data model and renders the UI but has no interactivity.

### Once you have a static application, what do you need to add?

A- After building the static version of the application, you should start adding interactivity since you have a library of components.

### What are the three questions you can ask to determine if something is state?

A-

* Is it passed in from a parent via props? If so, it probably isn’t state.
* Does it remain unchanged over time? If so, it probably isn’t state.
* Can you compute it based on any other state or props in your component? If so, it isn’t state.

### How can you identify where state needs to live?

A- The state should be where every a function should be called to update/do something based on that state, generally it sits on a parent.


## Things I want to know more about

- Most of my questions are already answered, but I would like to learn more about JSON files.



[Go Back](https://musaabshalaldeh.github.io/reading-notes/)