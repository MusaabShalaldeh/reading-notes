# Classes and Objects

Classes and Objects are not that different from Classes and Objects in other languages, so what are they exatly ?

Objects are a set of variables and functions put into a single entity. Objects get their variables and functions from classes so  Classes are essentially a template to create your objects.

Example of a simple class:
```Python
class MyClass:
    variable = "blah"

    def function(self):
        print("This is a message inside the class.")
```
Also, we can access class functions and methods in order to execute code inside them, and that is extremly useful in Object Oriented Programming, so how can we access an variable or a method inside a class/object ?

To access an variable or a method inside a class, we simply use notation objName.Variable / objName.method()

Example Code:
```Python
class MyClass:
    variable = "blah"

    def function(self):
        print("This is a message inside the class.")

myobjectx = MyClass()

print(myobjectx.variable)
```
which would end up printing the string "Blah"

# Thinking Recursively

What is thinking recrusively ? and why is it useful ?

Thinking Recrusively essentionally breaking down problems into smaller chucks that are easier to solve.

There is a fun example of thinking recruisevly using Santa Calus example which is:

(this is the typical structure of an iterative algorithm)
that Santa Claus has a list of houses he loops through. He goes to a house, drops off the presents, eats the cookies and milk, and moves on to the next house on the list. Since this algorithm for delivering presents is based on an explicit loop construction, it is called an iterative algorithm.


(This is the typical structure of a recursive algorithm)
but since Santa is old and he has many elves that he can ask for help, which would look like;

1-Appoint an elf and give all the work to him
2-Assign titles and responsibilities to the elves based on the number of houses for which they are responsible:
> 1 He is a manager and can appoint two elves and divide his work among them 
= 1 He is a worker and has to deliver the presents to the house assigned to him


### Recrusive Functions in Python

So what is a recrusive function ?

It is a that function will continue to call itself and repeat its behavior until some condition is met to return a result.

one of the most famous exmaples of this is the fibonacci:
```Python
def fibonacci(n):
    if n == 0:
      return 0
    elif n == 1:
      return 1
    else:
      return fibonacci(n + 1) + fibonacci(n + 2)
```


### Recursive Data Structures in Python

What does make a data structure recrusive ?

A data structure is recursive if it can be deﬁned in terms of a smaller version of itself.

Example Code:
```Python
def list_sum_recursive(input_list):
    # Base case
    if input_list == []:
        return 0

    # Recursive case
    # Decompose the original problem into simpler instances of the same problem
    # by making use of the fact that the input is a recursive data structure
    # and can be deﬁned in terms of a smaller version of itself
    else:
        head = input_list[0]
        smaller_list = input_list[1:]
        return head + list_sum_recursive(smaller_list)
 
  list_sum_recursive([1, 2, 3])

```


# Pytest Fixtures and Coverage

Why Fixtures ?

When you're writing tests, you're rarely going to write just one or two. Rather, you're going to write an entire "test suite", with each test aiming to check a different path through your code. In many cases, this means you'll have a few tests with similar characteristics, something that pytest handles with "parametrized tests".

But in other cases, things are a bit more complex. You'll want to have some objects available to all of your tests. Those objects might contain data you want to share across tests, or they might involve the network or filesystem. These are often known as "fixtures" in the testing world, and they take a variety of different forms.

To define a fixture, we use a combination of the pytest.fixture decorator, along with a function definition as the next example does:

```Python
def reverse_lines(f):
   return [one_line.rstrip()[::-1] + '\n'
           for one_line in f]
```

What is Coverage ?

A tool for measuring code coverage of Python programs. It monitors your program, noting which parts of the code have been executed, then analyzes the source to identify code that could have been executed but was not. Coverage measurement is typically used to gauge the effectiveness of test

[Go Back](https://musaabshalaldeh.github.io/reading-notes/)