# Testing and Modules


### Unit Tests & TDD with Python

What is TDD ?

TDD stands for Test-Driven Development which is a programming strategy mainly done by using Unit tests which are pieces of code to exercise the input, the output and the behaviour of your code and they can be written at any time either,Also TDD encourages developers to focus on software design first then writing actual code to help prevent problems and bugs that could be potentially faced down the line.

What are TDD steps in order ?

1- Desgin the software.
2- Write few tests.
3- Write actual code.
4- Run tests and make sure that the code is running fine.

Main key points to keep in mind about TDD Strategy:

* The greatest advantage about TDD is to craft the software design first.
* Your code will be more reliable: after a change you can run your tests and be in peace.
* Beginning may be hard, but with practice it is going to be easier.



### If name equals main


In code:
```
if __name__ == “__main__”
```

What does it do ?

When the python interpreter is running a module as the main program, it sets the special __name__ variable to have a value “__main__”. If this file is being imported from another module, __name__ will be set to the module’s name. Module’s name is available as value to __name__ global variable. 

Why Do we need it ?

To know if the code is executed directly from the module it self or from the script that imports that module.

What are its advantages ?

1- Every Python module has it’s __name__ defined and if this is ‘__main__’, it implies that the module is being run standalone by the user and we can do corresponding appropriate actions.

2- If you import this script as a module in another script, the __name__ is set to the name of the script/module.

3- Python files can act as either reusable modules, or as standalone programs.

4- if __name__ == “main”: is used to execute some code only if the file was run directly, and not imported.


### Recursion

What is recursion ? 

It is the process in which a function calls itself repeatedly in order to solve an algorithm.

Code Example:

```
int fact(int n)
{
    if (n < = 1) // base case
        return 1;
    else    
        return n*fact(n-1);    
}
```


[Go Back](https://musaabshalaldeh.github.io/reading-notes/)