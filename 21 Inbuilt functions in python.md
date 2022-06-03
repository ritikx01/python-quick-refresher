1. Lambda function.
Lambda function is a temporary, small and anonymous function.
```python
sqr = lambda x: x*x
print(sqr(2))
```
> 4
Lambda function evaluates the condition and returns the values.
```python
grt = lambda a,b : a if a > b else b
grt(5,9)
```
>9

*Note*: In the above code, printing grt directly (print(grt)) or using lambda function inside print ( print(lambda a,b : a if a > b else b) ) is 
equal to directly printing a function without calling it. Ex:
```python
def sqr(n):
    return n * n
print(sqr)
```


2. Map function ( map() ) takes two arguments, a funtion and a list. It then iterates the list over that function. To get the output in list 
format, we would have to use list() function.
```python
# Convert data types in a number from str to int.
nums_list = ["1", "2", "5"]
new_list = list(map(int, nums_list))
print(new_list)
```
> [1, 2, 3]
```python
def sqr(n):
    return n*n

num_list = [1, 4, 9, 3]
new_list = list(map(sqr, num_list))
print(new_list)
```
> [1, 16, 81, 9]

3. filter function() also takes two arguments, a function and a list, it also iterates the list over that function but returns only those elements
that evaluate to true.
```python
def less_than_10(n):
    if n < 10:
        return True
    return False

num_list = [5, 11, 56, 4, 9]
new_list = list(filter(less_than_10, num_list))
print(new_list)
```
> [5, 4, 9]

### Implementation of above using lambda function
1. 
```python
num_list = [1, 4, 9, 3]
new_list = list(map(lambda e: e*e, num_list))
print(new_list)
```
> [1, 16, 81, 9]

2. 
```python
num_list = [5, 11, 56, 4, 9]
new_list = list(filter(lambda e: e < 10, num_list))
print(new_list)
```
> [5, 4, 9]

