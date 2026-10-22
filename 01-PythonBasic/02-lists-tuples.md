## Tuples
- tuples are ordered sequences


```python
tuple1 =('kevin', 10, 1.2)
print(tuple1[0])
print(tuple1[1])
print(tuple1[-3])
```

    kevin
    10
    kevin
    

#### Concatenating tuples


```python
tuple1 =('kevin', 10, 1.2)
tuple2 = tuple1 + ('ph4n', 144)
print("Output:", tuple2)
# dw, "Output" is just there for the love of the game
```

    Output: ('kevin', 10, 1.2, 'ph4n', 144)
    

#### Slicing tuples


```python
tuple2 = ('kevin', 'phan', 10, 144, 1.2)
print("Output:",tuple2[0:3])
# the last index (3) is one larger than the index you want
```

    output: ('kevin', 'phan', 10)
    

#### sorted()


```python
tuple1 = (2, 6, 1, 0, 3, 7, 8, 8, 8)
tuple1_sorted = sorted(tuple1)
print("Output:", tuple1_sorted)
```

    Output: [0, 1, 2, 3, 6, 7, 8, 8, 8]
    

#### Nesting tuples


```python
Tuple1 = (1, 2, (3,4), ('kevin', 'phan'))
# So Tuple1[2] = (3,4)
# -> Tuple1[2][1] = 4
print(Tuple1[2][1])
```

    4
    

#### min() and max()


```python
num = (5,10,15,20,25,30)
print("min:", min(num))
print("max:", max(num))
```

    min: 5
    max: 30
    

#### sum()


```python
num = (5,10,15,20,25,30)
print("sum:", sum(num))

```

    sum: 105
    

---
## Lists
- are also ordered sequences
- however, they use square brackets instead


```python
List1 = ['kevin', 10, 1.1, (12, 13)]
```

#### del() (which means delete an item from the list)


```python
List1 = ['kevin', 10, 11]
del(List1[1])
print(List1)
```

    ['kevin', 11]
    

#### using split() to convert string to list


```python
A = "kevin phan".split()
print(A)
```

    ['kevin', 'phan']
    


```python
A = "kevin,phan,is,handsome".split(",")
print(A)
```

    ['kevin', 'phan', 'is', 'handsome']
    

#### append() to add ONE element to the end of a list


```python
List1 = [1,2,3,4,5]
List1.append(6) 
print(List1)
```

    [1, 2, 3, 4, 5, 6]
    

#### copy() to basically copy a list


```python
List1 = [1,2,3,4,5]
List2 = List1.copy()
print(List2)
```

    [1, 2, 3, 4, 5]
    

#### practice


```python
A=[1,2,3] + [1,4,7]
print(A)
```

    [1, 2, 3, 1, 4, 7]
    


```python
A = [1]
A.append([2,3,4,5])
print(A)
len(A)
```

    [1, [2, 3, 4, 5]]
    




    2




```python
my.profile = ('male', 18, "CS", 'engineering', 'HCMC')
len(my.profile)
```




    5


