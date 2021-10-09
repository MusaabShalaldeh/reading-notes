# Operators & Loops.

### Operators:

Operators in programming languages are symbols that tell the compiler to perform specific mathematical, relational or logical operation.

There are many Operators, but I am going to talk about 2 with example code:

* Assignment Operator 

-Assign values to varriables.
``` 
var myVariable = 5;
```
* Subtraction Operator

-Subtracts from the value the specified amount.
``` 
myVariable -= 5;
```
[Full Documentation](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)

### Loops:

Loops repeat a sequence of instructions until a specific condition is met, which is very useful in programming to help do repeated actions easily.

There are 2 main types of loops.

1. While Loops
```
var conditon = true;

while(conditon === true)
{
  //execute code until true becomes false.
}
```
Mainly used in situations when you don't know exactly when the condtion will end, but eventually it will.

2. For Loops
```
var numberOfLoops = 5;

for(var i = 0; i < numberOfLoops; i++)
{
  //execute this block of code depending on the number of loops which is in this case is 5
  console.log("hey! person number "+i)
}
```
Mainly used when you know when the condtion will end or specify how many times should it run.


[Go Back](https://musaabshalaldeh.github.io/reading-notes/)