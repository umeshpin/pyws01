## The os and sys modules.
----- 
# os Module

The OS module in Python provides functions for interacting with the operating system. OS comes under Python’s standard utility modules. This module provides a portable way of using operating system-dependent functionality. The *os* and *os.path* modules include many functions to interact with the file system.

```python
import os 
cwd = os.getcwd() 
print("Current working directory:", cwd) 
```
To list Files and directories in path

```python
path = "/"
dir_list = os.listdir(path)
print("Files and directories in '", path, "' :")
print(dir_list)
```

# sys module  

The sys module in Python provides various functions and variables that are used to manipulate different parts of the Python runtime environment. It allows operating on the interpreter as it provides access to the variables and functions that interact strongly with the interpreter


```python
import sys
print(sys.version)
```
Now Try 

```python
import sys
sys.stdout.write('Hi all')
```

```python
print(sys.path)
```
 
```python
print(sys.modules)
```
# Random numbers. 


The random() method in random module generates a float number between 0 and 1.

```python
import random
n = random.random()
print(n)
```
The randint() method generates a integer between a given range of numbers.    

```python
import random
n = random.randint(0,22)
print(n)           
```
Generating a List of numbers Using For Loop
```python
import random
randomlist = []
for i in range(0,5):
    n = random.randint(1,30)
    randomlist.append(n)
print(randomlist)
           
```



