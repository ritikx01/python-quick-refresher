Some examples of functions we have used already are print(), type(), str().

## Defining a function
```python
def greeting(name, department):                # Function greeting is defined with arguments name and department
	print("Welcome," + name)                   # Appropriate indentation before the contents of function
	print("You are part of " + department)
```

## Returning values
### Defining function
```python
def area_triangle(base, height):
	return base*height/2                       # We could've also stored the value of base*height/2 and returned it
```
### Calling function
```python
area1 = area_triangle(4,5)
print(area1)
area2 = area_triangle(7,3)
print(area2)
```
The output:
```
10.0
10.5
```

## Returning nostring from a function
```python
def greet(name):
	print("Welcome," + name)
```
Calling it
```python
result = greet("Ritik")
print(result)
```
The output:
```
Welcome, Ritik										#Because of the print statement in the greet function
None												# variable result has value None because we didn't returned anything in the function
```

**None** - It is a special data type in python, used to indicate that strings are empty or that they returned nothing.
**Comments** - 1. Pound or Hash '#' symbol is used to denote single line comment.
								  2. Three quotation marks are used to denote multi line comments.Ex
```python
print("Hello visitor")
''' This is a multi            # Start of multi line comment
line comment example
in python
'''                            # End of multi line comment
print("Good to see you here")
```
								 