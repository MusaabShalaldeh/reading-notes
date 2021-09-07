# FUNCTIONAL PROGRAMMING




### What is functional programming?

A- Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data. (from wiki)

### What is a pure function and how do we know if something is a pure function?

A-
* It returns the same result if given the same arguments

* It does not cause any observable side effects

### What are the benefits of a pure function?

A- Pure functions are much easier to read and reason about. All relevant inputs and dependencies are provided as parameters, so no effects are observed that alter variables outside of the set of inputs. This means that we can quickly understand a function and its dependencies, just by reading the function's declaration

### What is immutability?

A- The state of not changing.

### What is Referential transparency?

A- a function that consistently yields the same result for the same input.




### What is a module?

A- A piece of code(another script) that has a certain  functionality.

### What does the word ‘require’ do?

A- Make a reference for another script in the project file.

### How do we bring another module into the file the we are working in?

A- By requiring it at the start of the script:
```
require('script_path");
```

### What do we have to do to make a module available?

A- By writing this line at the end of the module script:
```
module.export = whatever_function_to_be_public;
```



## Things I want to know more about

- Using modules.












[Go Back](https://musaabshalaldeh.github.io/reading-notes/)