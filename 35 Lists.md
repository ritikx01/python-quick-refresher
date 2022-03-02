This is a datatype similar to arrays. Square brackets [] are used to indicate lists.

Now we can use type,len or str in x to know about type,length of string or in a string is present in the list.

```python
x = ["Now", "we", "are", "talking"]
type(x)
<class 'list'>						#Output
len(x)
4									#Output
```

### Print part of a list
```python
print(x[0])
Now									#Output
print(x)
talking								#Output
print(x[1:3])
['we', 'are']

```

## Modifying the contents of a list
1. Adding element using "append" method
 ```python
fruits = ["Pineapple", "Banana", "Apple", "Melon"]
fruits.append("Kiwi")
print(fruits)
["Pineapple", "Banana", "Apple", "Melon", "Kiwi"]
```
Append always adds element to the end of the list
2. Adding element using "insert" method
```python
fruits.insert(0, "Orange")
print(fruits)
["Orange", "Pineapple", "Banana", "Apple", "Melon", "Kiwi"]
```
3. Remove using "remove" method
```python
fruits.remove("Melon")
print(fruits)
["Orange", "Pineapple", "Banana", "Apple", "Kiwi"]
```
4. Remove using "pop" method
```python
