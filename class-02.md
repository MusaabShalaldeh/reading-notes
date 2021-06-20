# Basics of HTML, CSS & JS


### Text in HTML

It is really important to have an organized text on your webpage, it helps readers understand the message you are trying to deliver, and for that very reason HTML offers plenty of methods to organize your text, most importantly the Headings and Paragraphs, also it gives you the ability to change how text looks to furthermore customize your text with Italic and Bold text styles.

As well as allowing you to have White Spaces(aka empty white space) to help organize text and make it easier to read, also you can make Lines Break to seperate 1 line text, which would be very helpful in some cases, and you can make important text look "strong" by using strong tag, and whats beautiful about HTML is that most of its tags are semantics and they tell you their function by just their tag name.


### CSS Basics

Lets start by asking what CSS is, CSS stands for Cascading Style Sheets, it describes how HTML elements are to be displayed on screen, also, it saves a lot of work. It can control the layout of multiple web pages all at once.

How does it work ?

it works by allowing the developer to manipulate specific tags, for example all h1 tags or specificed classes or certain ids which are manually given to blocks of code.

an code example would be:
```
h1{
    background-color: blue;
    text-align: center;
}
```
which would make all h1 tags have a blue background and align them to the center of the page.


### Javascript Basics


Lets start by comprehending what a script is, a script is a series of instructions that a computer can follow one-by-one. Each individual instruction or step is known as a statement.
Statements should end with a semicolon.

Those statements are made up of code blocks, and those code blocks can either contain variables, custom functions, variables are datatypes such as numbers, booleans(true/false), Arrays and strings(text).

to declare a variable, you simply do the following:
```
var customNumber = 5;
```
which assigns this variable to be a number and so on.


lets also not forget the operators as they are really important because they allow programmers to
create a single value from one or more values and expressions rely on them, aswell as Arithmetic operators which gives us evenmore ability to add/subtract etc.. values at ease.


### Loops & Decision making

Loops repeat a sequence of instructions until a specific condition is met, which is very useful in programming to help do repeated actions easily.

There are 2 types of loops, but for decision making we will be using While loop:

While Loops are used whenever we don't know when will the operation will end, best used for **Decision making**, for example:
```
let myBool = true;
let myNumber = 0;
while(myBool)
{
    //keep deciding a an outcome depending on the value
    myNumber++;
    console.log("im bored, im gonna keep poking you");
    if(myNumber > 50)
    {
        myBool = false;
        console.log("I Changed my mind, I will stop now.")
    }
}
```
in the example above, it shows how we made the computer think for its own and decide to either stop or keep annoying the user.



[Go Back](https://musaabshalaldeh.github.io/reading-notes/)