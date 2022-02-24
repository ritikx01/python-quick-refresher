## Data Types
1. Ex- str, int, float
2. Check for datatype:
	1.  `print(type("a"))`    Out: `<class 'str'>`
	2.  `print(type(2))`    Out: `<class 'int'>`
	3.  new_list[]
	      `print(type(new_list))`    Out: `<class 'list'>`
3. Operation between two different Data Types results in `TypeError`
## Variables
Variables are names given to ceratin values in the program. 
Ex-
1. length = 10
2. width = 2
3. area = length \* width

### Variables naming convention
1. Don't use keywords or functions that python reserves for it's own. This may result in a conflict. Ex- break, True, and, class
2. Don't use spaces in between variable names
3. Must start with a letter or an underscore(\_)

## Type Conversion
This simply means to change one data type to another.
1. Implicit conversion - The interpreter automatically converts one data type into another.
`print(7+8.5)` = 15.5 			(7 is of type int and 8.5 is of type float. The result is implicitly converted to float)
2. Explicit conversion
```python
year = 2022          # Data type Integer
year1 = str(2022)    # Using str() function to change the type to String
print(type(year))
print(type(year1))
```
The output:
```
<class 'int'>
<class 'str'>
```