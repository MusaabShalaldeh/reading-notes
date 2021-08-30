# Passing Functions as Prop

# React Lists & Keys

### Q-What does .map() return?

A- It returns a new array based on the array that this function was called on.

### If I want to loop through an array and display each value in JSX, how do I do that in React?
A- Example Code from [React Documentation](https://reactjs.org/docs/lists-and-keys.html):
```
const numbers = [1, 2, 3, 4, 5];
const listItems = numbers.map((number) =>
  <li>{number}</li>
);

ReactDOM.render(
  <ul>{listItems}</ul>,
  document.getElementById('root')
);
```
### Each list item needs a unique ____.

A- Key.

### What is the purpose of a key?

A- Keys are used to React to identify which items in the list are changed, updated, or deleted.



# Spreader Operator

### What is the spread operator?

A- The spread operator is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.

### List 4 things that the spread operator can do.

A-
* Concatenating or combining arrays
* Using Math functions
* Adding to state in React
* Converting NodeList to an array

### Give an example of using the spread operator to combine two arrays.

```
const arr1 = [a,b,c]
const arr2 = [d,e,f]
const arr3 = [...arr1, ...arr2]
console.log(arr3) => [a,b,c,d,e,f]
```

### Give an example of using the spread operator to add a new item to an array.

```

const arr1 = ['2','5','7']
const arr2 = ['8',...arr1]
console.log(arr2) => ['8','2','5','7']
```

### Give an example of using the spread operator to combine two objects into one.

```
let person = {
    firstName: 'John',
    lastName: 'Doe',
    age: 25,
    ssn: '123-456-2356'
};


let job = {
    jobTitle: 'JavaScript Developer',
    location: 'USA'
};

let employee = {
    ...person,
    ...job
};

console.log(employee); which will output:
{
    firstName: 'John',
    lastName: 'Doe',
    age: 25,
    ssn: '123-456-2356',
    jobTitle: 'JavaScript Developer',
    location: 'USA'
}
```


# How to Pass Functions Between Components

### In the video, what is the first step that the developer does to pass functions between components?

A- Add a new prop in the render function and call it on the reciving end.

### In your own words, what does the increment function do?

A- A custom function that increases a number whenever its called.

### How can you pass a method from a parent component into a child component?

A-  
* In the parent component, create a callback function. ...

* Pass the callback function to the child as a props from the parent component.

* The child component calls the parent callback function using props and passes the data to the parent component.

### How does the child component invoke a method that was passed to it from a parent component?

A- By Running this code:
```
    this.props.increment(this.props.name)
```




## Things I want to know more about

-Using events with react and making an interacable webpage.

-Putting state variables to more use in a complex webpage.



[Go Back](https://musaabshalaldeh.github.io/reading-notes/)