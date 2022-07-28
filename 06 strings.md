# No strings attached

String can be expressed in Python by several ways. They can be enclosed in single quotes or double quotes:
One thing to note is that in a string, a single backslash at the end of the line indicates that the string is continued in the next line, but no newline is added. 

For example

```python
"This is the first sentence.\ This is the second sentence."'This is the first sentence. This is the second sentence.'
```
Note the operator ".\" used to enter the string in the next line without changing its structure

Try some string operations using Python
```python
stri = 'programming' 
print(stri)		# Prints complete string 
print (stri[0])		# Prints first character of the string 
print (stri[2:5])	# Prints characters starting from 3rd to 6th 
print (stri[2:])		# Prints string starting from 3rd character
```

Concatenation and repetition in python

The plus (+) sign is the string concatenation operator, and the asterisk (*) is the repetition operator.

```python
str1 = 'Enjoy' 
str2 = 'Python' 
print (str1+str2)		# combine two strings str1 and str2 
print (str1*10)		# Prints string ten times
```

We can find a particular string by ".find" method
```python
S = 'yyyyyyyyyyyyyHIDDENaaaaaaaaaaaa' 
where = S.find('HIDDEN')
print(where)
```

isalpha() returns true if all characters in the string are alphabetic and there is at least one character, false otherwise.
```python
print('allstring'.isalpha() )
```

isdigit() returns true if all characters in the string are digits
```python
print('123'.isdigit() )  
```

isspace() returns true if there are only whitespace characters
```python
print('1  23'.isspace() ) 
```


# Malayalam in Python

```python
import unicodedata
mal=u'എനിക്ക് മലയാളം അറിയാം'
mal=mal.encode('utf-8').decode('utf-8')
print(mal)
```

Lets make Working day a Holiday

```python
S = 'Workingday' 
S = S.replace('Working', 'Holi')
print(S)
```

# f-strings (Valid from Python 3.6 onwards)

```python
me = "Umesh"
program = "FDP on Python"
print(f"Hi! I am {me} and I welcome all of you to {program}!")
```


