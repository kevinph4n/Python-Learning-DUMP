### Comparison


```python
i = 1
i >= 7 # greater or equals
```




    False




```python
i = 12
i != 10
# != means "not equals"
# -> it's true that 12 isn't = 10
```




    True



- this goes the same to strings


```python
"kevin" == "ph4n" # this a false
"kevin" != "ph4n" # this a true
```




    True



---
### Branching

#### 1/ if


```python
age = 18
if (age > 21):
 
 print('you may drink alcohol')

print("keep it going")

# -> if the statement is False -> it passes to the next
```

    you can't drink alcohol
    

#### 2/ else


```python
age = 18
if (age > 21):
    print("you may drink alcohol")

else:
    print("get out")

print("keep it going")

# the system checks if the "if (age > 21)" is true or false -> processes the else
# whether if the if condition is true or false, "keep it going" will still be there
```

    get out
    keep it going
    


```python
age = 22
if (age > 21):
    print("you may drink alcohol")

else:
    print("get out")

print("keep it going")
```

    you may drink alcohol
    keep it going
    

#### 3/ elif (short for else if)


```python
age = 21
if (age > 21):
    print("you may drink alcohol")

elif (age == 21):
    print("you may drink it...only this time okay?")

else:
    print("get out")

print("keep it going")
```

    you may drink it...only this time okay?
    keep it going
    

---
### Logic Operators

#### 1/ or
- A: False | B: False | A or B: False
- A: False | B: True  | A or B: True
- A: True  | B: True  | A or B: True


```python
born_year = 2008
if (born_year < 2000) or (born_year > 2009):
 print("kevinph4n was born in the 90s or 2010s")

else:
    print("kevinph4n was born in 2000s")
```

    kevinph4n was born in 2000s
    

#### 2/ and
- A: False | B: False | A and B: False
- A: False | B: True  | A and B: False
- A: True  | B: False | A and B: False
- A: True  | B: True  | A and B: True


```python
born_year = 2008
if (born_year > 2007) and (born_year < 2009):
    print("kevinph4n was born in 2008")
```

    kevinph4n was born in 2008
    
