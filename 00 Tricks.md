# Python tricks to code faster.

1. Printing a list.
    `a = [1, 2, 3, 4, 5]`
    1. `print(*a)`			# This gives all the elements as arguments. \* is the unpacking operator.
    2. `print(' '.join(a))`

2. Find longest string in a list.
    ```python
    a = ['I', 'like', 'Python']
    print(max(a, key=len))
    python				# Output
    ```
3. Iterate over list and keep count of index.
    ```python
    a = ['Hello', 'I', 'am', 'Ritik']
    for i, j in enumerate(a):
       print(i, j)

    0 Hello				# Output
    1 I
    2 am
    3 Ritik
    ```
    Enumerate functi
