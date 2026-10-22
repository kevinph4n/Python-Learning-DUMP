#### range(N)



```python
range(5)
# 0, 1, 2, 3, 4 (the last number is lower than 1)
```




    range(0, 5)



#### For loops
- Loops: perform a task over and over


```python
for x in ['A', 'B', 'C']:
    print(x +'A')

# The list is ['A', 'B', 'C']
# for function will concatenate each of them with:
# 1st: x = 'A'
# 2nd: x = 'B'
# ... -> 'A' + 'A' = 'AA' and so on
```

    AA
    BA
    CA
    


```python
for i, x in enumerate(['A', 'B', 'C']):
    print(i,x)

# with enumerate, it's just like [(0, 'A'), (1, 'B'), (2, 'C')] (just e.g)
# 1st: i = 0; x = 'A' -> print(i, x) = 0 A
# ... and so on
```

    0 A
    1 B
    2 C
    

#### While loops
- While loops: will only run if a condition is met


```python
x = 5
while x != 2:
    print(x)
    x = x-1
```

    5
    4
    3
    


```python
colors = ['red', 'red', 'blue', 'red', 'green']
new_colors=[]
i = 0 # the index starts at 0

while(colors[i]=='red'): # this statement will repeatedly execute the statements
    # until the condition inside the bracket is False
    new_colors.append(colors[i]) 
    # append from the list 'squares' to the list "news_quares"
    i = i + 1
```
