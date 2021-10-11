# Reading & Writing files with Python


Reading and Writing files is one of the most common things that are done in Python due to many reasons such as reading raw data, reading a complicated server log and many more.

### What is a file ?

A file is a contiguous set of bytes used to store data. This data is organized in a specific format and can be anything as simple as a text file or as complicated as a program executable.

Also, each file is made up of 3 components:

1-Header: metadata about the contents of the file (file name, etc..)

2-Data: contents of the file as written by the creator or editor

3-End of file (EOF): special character that indicates the end of the file

### How can we read or write to a file  with python ?

-Reading a file:

with python it is very simple to read a file, all we gotta do is just to provide a path to open() function and we should be good to go.

Example Code:
```Python
file = open('list_of_foods.txt')
print(file.readlines())
```
*Note:* that a file must be closed after finishing reading it so that we clear up the memory and save on resources.

The open() function also can take an optional argument such as:

1- 'r' Open for reading (default)

2- 'w' Open for writing, truncating (overwriting) the file first

3- 'rb' or 'wb'	Open in binary mode (read/write using byte data)

-Write a file:

It is just as simple to write to a file, all we have to do is make sure to open a file is opened with the correct parameters

Example Code:
```Python
file = open('list_of_foods.txt','w')

file.write("adding a new line to that")
```


# Exceptions in Python


### Exceptions versus Syntax Errors

Syntax errors are errors that occur when rules of the used programming language are not followed correctly thus creating an error which forces the program to shut down, on the other hand, Exception errors occur when the code it self is not giving an correct out put, mainly used in TDD process of programming.


### How can we raise an Exception error ?

To raise an exception error We can use raise to throw an exception if a condition occurs. The statement can be complemented with a custom exception.

Example Code:
```Python
x = 10
if x > 5:
    raise Exception('x should not exceed 5. The value of x was: {}'.format(x))
```
When you run this code, the output will be the following:

```Python
Traceback (most recent call last):
  File "<input>", line 4, in <module>
Exception: x should not exceed 5. The value of x was: 10
```


Also, there is something called **The AssertionError Exception** which we use to  assert that a certain condition is met. If this condition turns out to be True, then that is excellent! The program can continue. If the condition turns out to be False, you can have the program throw an AssertionError exception.







[Go Back](https://musaabshalaldeh.github.io/reading-notes/)