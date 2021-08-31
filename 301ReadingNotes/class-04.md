# React and Forms




# React Docs - Forms

### What is a ‘Controlled Component’?

A- A controlled component is a component that renders form elements and controls them by keeping the form data in the component's state

### Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

A- we should update the state with the user's responses as soon as they enter them, because react handles data whenever they are updated.

### How do we target what the user is entering if we have an event handler on an input field?

A- 
* Create an arrow function called handleInputChange which accepts event as its own argument within the App component.

* Within the function, use the passed in event parameter to get the target input element; from the target get the value and name of the input element.


# The Conditional (Ternary) Operator Explained


### Why would we use a ternary operator?

A- To simplify if/else statements that are used to assign values to variables.

### Rewrite the following statement using a ternary statement:

A-
```
const x = 1;
const y = 2;
console.log((x===y) ? console.log(true) : console.log(false));
```




## Things I want to know more about

-Using Forms with React bootstrap

-Customizing Forms with bootstrap

-Put condtional rendering to use







[Go Back](https://musaabshalaldeh.github.io/reading-notes/)