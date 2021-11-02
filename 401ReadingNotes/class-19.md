# Regular Expression in Python

### What is Regular Expressions ?

- Regular Expressions are a sequence of characters used to check whether a pattern exists in a given text (string) or not.

### Examples of What Regular Expressions are used for:

1. Validate the format of email addresses or passwords during registration.

2. Parsing text data files to find, replace, or delete certain string.

3. Manipulating textual data, which is often a prerequisite for data science projects involving text mining


### How to use Regular Expressions ?

* Start by importing the Regular Expressions module
```python
import re
```

* lets check if a provided word starts with a and ends with s:

```python
pattern = '^a...s$'
test_string = 'abyss'
result = re.match(pattern, test_string)

if result:
  print("Search successful.")
else:
  print("Search unsuccessful.")	
```

which will print out search successful as it found a match using the pattren.


# Shutil


### What is Shutil ?

Its a python module that includes high-level file operations such as copying and archiving.


### Why use Shutil ?

To accomplish tasks, such as: copying, moving, or removing directory trees automatically.

### How to use Shutil ?

Just as any other module we have to import it first as well as importing os module

```python
# importing os module
import os
 
# importing shutil module
import shutil
```


```python
# Python program to explain shutil.copyfile() method
# path
path = '/home/User/Documents'
 
# List files and directories
# in '/home/User/Documents'
print("Before copying file:")
print(os.listdir(path))
 
 
# Source path
source = "/home/User/Documents/file.txt"
 
# Destination path
destination = "/home/User/Documents/file(copy).txt"
 
# Copy the content of
# source to destination
dest = shutil.copyfile(source, destination)
 
# List files and directories
# in "/home / User / Documents"
print("After copying file:")
print(os.listdir(path))
 
# Print path of newly
# created file
print("Destination path:", dest)
```

which will end up copying the text file from documents to the same directory but under a different name(file(copy).txt) and we can apply this to any destination on our operating systems.


[Go Back](https://musaabshalaldeh.github.io/reading-notes/)