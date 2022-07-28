To program decisions and do different things depending on different situations can be achieved by the control statements.  There are three control flow statements in Python - if, for and while.

## The if statement:

The  if statement contains a logical expression using which data can be compared, and a decision is made based on the result of the comparison.

The syntax of the if statement is:
```python
if expression:
         statement(s)   // Note the indentation 
```
Here if statement, condition is evaluated first. If condition is true, the statement(s) block are executed. Otherwise, the next statement following the statement(s) block is executed.
```python
inti= int(input('Enter One or Two : '))
if inti==1:
   print("Value of integer, int is 1")
if inti==2:
   print("Value of integer, int is 2")
```
   
## The else Statement:

An else statement can be combined with an  if statement. An else statement contains the block of code that executes if the conditional expression in the if statement resolves to 0 or a false value. 
Try 

```python
inti= int(input('Enter One or Two : '))
if inti==1:
   print("Value of integer, inti is 1")
else:
   print("I told you to enter 1. You have entered another value")
```

## The while Loop:

The while loop is one of the looping constructs available in Python. The while loop continues until the expression becomes false. The expression has to be a logical expression and must return either a true or a false value
```python
count = 0 
while (count < 9):
    print('line number:', count )
    count = count + 1
print("Finished!" )
```

The for Loop:

The for loop in Python has the ability to iterate over the items of any sequence, such as a list or a string.

Syntax of For loop
```python
for iterating_var in sequence:
  statements(s) 
```
Try the following code
```python
fruits = ['banana', 'apple',  'mango'] 
for index in range(len(fruits)):         
  print('Current fruit :', fruits[index]) 
print("No more fruits!")
```

