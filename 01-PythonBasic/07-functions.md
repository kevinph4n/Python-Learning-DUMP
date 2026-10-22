### Functions
- is just a piece of code you can reuse (after making ur own or using others')
- Python has many built-in Functions


```python
# e.g. f1 -> f2 -> f2 -> f1
def f1(input):
    """ add 1 to input """
    output = input + 1
    return output
# when we call function 1 (f1). we pass an input to the function
# these values are passed to all lines of code u wrote
# this returns 'output' which is a value -> this value can be used


def f2(input):
    """ add 2 to input """
    output = input + 2
    return output
# when we call a new function 2 (f2), the value is passed to another set of lines of code
# then a value is returned
# the process is repeated, passing the values to the function you call

# -> these functions can be saved and reuse, or use others' functions
```

### Python Built-in Functions
#### 1/ Len


```python
len(['A','B',1])
```




    3




```python
len([sum([1,1,1])])
```




    1




```python
marks = [8.5, 8.0, 9.0, 5.5, 6.5]
marks_len = len(marks)
print(marks_len)
```

    5
    

#### 2/ Sum


```python
marks = [8.5, 8.0, 9.0, 5.5, 6.5]
sum_marks = sum(marks)
print(sum_marks)
```

    37.5
    

#### 3/ Sorted vs Sort


```python
A = [2, 4, 6, 7]
A.sort()
print(A)
```

    [2, 4, 6, 7]
    


```python
marks = [8.5, 8.0, 9.0, 5.5, 6.5]
sorted_marks = sorted(marks)
print(sorted_marks)
# In this case, sorted_marks is a new list
```

    [5.5, 6.5, 8.0, 8.5, 9.0]
    


```python
marks = [8.5, 8.0, 9.0, 5.5, 6.5]
marks.sort()
print(marks)
# In this case, the list marks just got updated, no new list was created
```

    [5.5, 6.5, 8.0, 8.5, 9.0]
    

---
### Making Functions


```python
def add1(x):
    ''' add 1 value to x'''
    y = x + 1
    return y
```

#### 1/ Multiple parameters


```python
def mult(x, y):
    z = x * y
    return z
# -> z = x x y (if it is x = 2, y = kevin -> z = kevin kevin)
```


```python
def kevinph4n():
    print('Kevin Phan')
print(kevinph4n())
```

    Kevin Phan
    None
    

#### 2/ Functions performing multiple tasks


```python
def add1(x):
    y = x + 1
    print(x, 'plus 1 is ', y)
    return y
```

    3
    

#### 3/ Loops in Functions


```python
def print_function(X):
    for x in X:
        print(x + '1')
print_function(['a', 'b', 'c'])
```

    a1
    b1
    c1
    


```python
def printMarks(marks):
    for i,s in enumerate(marks):
        print('Marks', i, "The mark is ", s)

marks = [8.5, 8.0, 9.0, 5.5, 6.5]
printMarks(marks)
```

    Marks 0 The mark is  8.5
    Marks 1 The mark is  8.0
    Marks 2 The mark is  9.0
    Marks 3 The mark is  5.5
    Marks 4 The mark is  6.5
    

#### 4/ Collecting arguments


```python
def Marks (*marks):
    for mark in marks:
        print (mark)

Marks(8.5, 8.0, 5.5)
```

    8.5
    8.0
    5.5
    

#### 5/ Scope


```python
def A(x):
    x = x + "A"
    print(x)
    return x

x = 'B'
z = A(x) # a variable defined in the global scope is called a global variable
```

    BA
    


```python
def Apocalypse(x):
    print(Likes)
    return (Likes + x)

Likes = 100
Z = Apocalypse(1)
print(Likes)
```

    100
    100
    


```python
len(['A','B',1])
```




    3


