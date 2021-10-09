# Problem Domain, Objects, and the DOM


### Problem Domain

Problem domain is an engineering term referring to all information that defines the problem and constrains the solution (the constraints being part of the problem).
###### _Definition from google searching_


As most of people who are new to learning programming said that the hardest part of learning programming is the Problem Domain, and as a reader, you would ask why so lets answer that, because its like answering a question that you don't know, so before writing code, you must consider all possible outcomes and have an answer to them.


Also, understanding the problem domain helps you as a developer to spend less time working on a project, as in if you spent alot of time planning all possible cases of a code scenario and wrote it once than understanding half the picture and rewriting code over and over.



### Object Literals

Object Literals are the values that can be properties and functions, mostly used to define classes which are very helpful when having a case where you need to store multiple attributes/values/functions on a single object.

Example Code:
```
var greeting = {
    fullname: "Michael Jackson",
    greet: (message, name) => {
        console.log(message + " " + name + "!!");
    }
};
```
and to use or log those values we do this:
```
console.log(greeting.fullname);
//call greet function thats inside the greet variable .
greeting.greet("Greeting", greeting.fullname);

// what console logs:
Michael Jackson
Greeting Michael Jackson!!
```

### The DOM

DOM stands for Document Object Model which is a model that specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window.
###### _Definition from Duckett Book About Js and JQeury_

Let's breakdown how it works in a short way, firstly, the browser represents the page using the Document Object Model, this model has four tree types which are:

1- Document Nodes.

2- Element Nodes.

3- Attribute Nodes.

4- Text Nodes.

Those nodes allow us to select their nodes by IDs, Classe, Tags or using the CSS selector with code, then we can manipulate those specific elements in order to have a real time interactable or configurable web page/ web applicate, such as changing the theme of your website, changing specific paragraph or button text and more.



[Go Back](https://musaabshalaldeh.github.io/reading-notes/)