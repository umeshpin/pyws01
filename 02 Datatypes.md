## Python Datatypes 
----- 
# list

A list contains items separated by commas and enclosed within square brackets. All the items belonging to a list can be of different data type.

```python
mylist = [ 'kerala', 257 , 2.23,0, 70.2 ] 
smalllist = [123, 'university']
print(mylist) 

```
Now Try 

```python
print(mylist[0])  # Prints first element of the list
print(mylist[1:3])  # Prints elements starting from 2nd to 4th
print(mylist[2:])   # Prints elements starting from 3rd element 
print(mylist + smalllist)  # Prints concatenated lists
```

# tuple 

A tuple is another sequence data type that is similar to the list. A tuple consists of a number of values separated by commas. Unlike lists, tuples are enclosed within parentheses.

The main differences between lists and tuples are: Lists are enclosed in square brackets and their elements and size can be changed but elements and size in tuple cannot be changed. Tuples can be considered as read-only lists.

Now lets have some experiments with list and tupple

```python
mylist = [‘kerala’, 257, 2.23,0, 70.2] 
mytuple = ('kerala', 257, 2.23,0, 70.2) 
```
Now Try 

```python
mylist[2]=0		# changes the third value in list 
mytuple[2]=0		# Invalid syntax with tuple
```

# Python Dictionary

Python’s dictionaries work like associative arrays or hashes found in Perl and consist of key-value pairs. Keys can be almost any Python type, but are usually numbers or strings. Values, on the other hand, can be any arbitrary Python object. Dictionaries are enclosed by curly braces.

Key -------------> value
User Name -------> Password

```python
mydict = {'james bond': '007', 'binary':'zero and one', 'year':2011}
```
To get values 
```python
mydict['james bond'] 
mydict['binary'] 
mydict['year’]

```
From values to keys [we will learn for loop] 
```python
mydict = {'james bond': '007', 'binary':'zero and one', 'year':2011}
def GetKey(val):
   for key, value in mydict.items():
      if val == value:
         return key
      return "key doesn't exist"
print(GetKey("007"))
```
      


# Operators in python

Python also uses similar operators to describe a mathematical operation. Addition, subtraction multiplication and division are described by +, -, *, / respectively. 

Operator      Description
1. ==              Checks if the value of two operands is equal or not, if yes, then condition becomes true
2. !=              Checks if the value of two operands are equal or not
3. <>              Checks if the value of two operands are equal or not
4. <              Checks if the value of left operand is less than the value of right operand
5. <=              Checks if the value of left operand is less than or equal to the value of right operand

# Membership Operators

One of key the features of Python programming language is that,  it has membership operators, which test for membership in a sequence, such as strings, lists, or tuples. There are two membership operators explained below:

Operator  
- in :   valuates to true, if it finds a variable in the specified sequence and false, otherwise.
- not in :    Evaluates to true, if it does not finds a variable in the specified sequence and false otherwise.

Try the following code

```python
mystring='Hello hai and bye' 
"hai" in mystring               # this will give whether string hai is present in the string str (TRUE or FALSE) 
```
Also Try 
```python
mystring.count("hai")            # this will count the number of hai present in the string
```

# Identity Operators

Identity operators compare the memory locations of two objects. There are two Identity operators explained below:

```python
a=5
b=6
c=5 
a is b 
a is c
```
# Input Functions

Input Functions is an interactive built-in function that communicate with user. Try the following command
```python
int= input('Enter an integer : ')
```
Using this command, user can assign value to variable int 
Noe try

```python
int 
```

## Methods in List
Lets use some Methods
```python
my_list=["Insta", "FB", "Youtube"]
my_list.append("Watsapp") 
print(my_list)
```
Append and Extend
```python
full_list = [1, 2, 3]
supply_list = [4, 5]
new_list=[6]
full_list.append(supply_list)
print(full_list)
supply_list.extend(new_list)
print(supply_list)
```
Some more trials
```python
full_list.pop()
print(full_list)
full_list.insert(1, 1.5)
print(full_list)
```





