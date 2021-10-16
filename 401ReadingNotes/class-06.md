#  Game of Greed 1



# How to use Random Module



### What is Random Module and When Should We Use It ?

-It is a module that provides access to functions that support many operations, It is used when we randomizes something, as in if we want the computer to pick a random number in a given range Pick a random element from a list or pick a random card from a deck or flip a coin etc.

### What are the methods that the Random Module provides ?

- Randint(or in other words, Random Intger/ Random Number) 

Example:

```Python
import random
print (random.randint(0, 5))

# output will be a random number from 1 to 5
```

- Random (generate a random float from 0.0 to 1.0)

Example:

```Python
import random
print(random.random() * 100)

# output will be a random float number
```

-Choice (Generate a random value from the input sequence)
Example:

```Python
import random
print(random.choice( ['red', 'black', 'green'] ))

# output will be a random item from the provided list
```

-Shuffle (the shuffle function, shuffles the elements in list in place, so they are in a random order)
Example:

```Python
from random import shuffle
x = [[i] for i in range(10)]
shuffle(x)
Output:
# print x  gives  [[9], [2], [7], [0], [4], [5], [3], [1], [8], [6]]
# result is different each time this code is run
```

-Randrange (Generate a randomly selected element from range(start, stop, step))
Example:

```Python
import random
for i in range(3):
    print (random.randrange(0, 101, 5))

# result will be 3 randomly generated numbers(between 1 and 101)
```


# What is Risk Analysis

To start off, Risk Analysis is the process of identifying the risks in applications or software that you built and prioritizing them to test. After that, the process of assigning the level of risk is done. The categorization of the risks takes place, hence, the impact of the risk is calculated.

### Why use Risk Analysis? 

In any software, using risk analysis at the beginning of a project highlights the potential problem areas. After knowing about the risk areas, it helps the developers and managers to mitigate the risks. When a test plan has been created, risks involved in testing the product are to be taken into consideration along with the possibility of the damage they may cause to your software along with solutions.


### Risk Identification

There are different sets of risks included in the risk identification process. Those are as follows:

* Business Risks: This risk is the most common risk associated with our topic. It is the risk that may come from your company or your customer, not from your project.

* Testing Risks: You should be well acquainted with the platform you are working on, along with the software testing tools being used.

* Premature Release Risk: a fair amount of knowledge to analyze the risk associated with releasing unsatisfactory or untested software is required

* Software Risks: You should be well versed with the risks associated with the software development process.

### Risk Assessment

In the risk analysis process, these steps prove to be the most important one. It is said that this step is way too complex and should be tackled with the utmost care. After risk identification, assessment has to be dealt programmatically. There are a few perspectives on risk assessment.

### The perspective of Risk Assessment

* 1-Effect – To assess risk by Effect. In case you identify a condition, event or action and try to determine its impact.

* 2-Cause – To assess risk by Cause is opposite of by Effect. Initialize scanning the problem and reach to the point that could be the most probable reason behind that.

* 3-Likelihood – To assess risk by Likelihood is to say that there is a probability that a requirement won’t be satisfied.



### How to perform Risk Analysis?
There are three steps:

* -Searching the risk

* -Analyzing the impact of each individual risk

* -Measures for the risk identified



# Test Coverage

-What is Test Coverage ? 

Test Coverage is a tool(or a process) used for finding untested parts of a codebase.

-How is it done ?

Its done by writing a suite of test functions that call the methods we want to test with different types of inputs to test every case.

-Notes about test coverage:

1- Its better to have few tests that execute different types of code rather than tens of test testing similar code.

2- There is always the possiblity of users finding bugs so don't sweat it, and just fix the code!


[Go Back](https://musaabshalaldeh.github.io/reading-notes/)