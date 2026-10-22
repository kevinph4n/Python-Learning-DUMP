### 1/ For a new line in the string: \n


```python
print("Hey \n baby")
```

    Hey 
     baby
    

### 2/ For a tab: \t


```python
print("Hey \t baby")
```

    Hey 	 baby
    


```python
print("Hey \\ baby")
```

    Hey \ baby
    

---
## **METHOD**
### 1/ .upper()


```python
A = "i can't help it but fall in love with you"
B = A.upper()
print(B)
```

    I CAN'T HELP IT BUT FALL IN LOVE WITH YOU
    

### 2/ .replace()


```python
A = "kevinph4n is handsome-ish"
B = A.replace('handsome-ish', 'handsome')
print(B)
```

    kevinph4n is handsome
    

### 3/ .find()    |   The output would be the first index of the string


```python
name = "Kevin Phan"
A = name.find('Phan')
B = name.find('Kevin')
print(A)
print(B)
```

    6
    0
    

### 4/ .title()


```python
name = "im a beast iykyk"
A = name.title()
print(A)
```

    Im A Beast Iykyk
    

---
### PRACTICES

#### 1/


```python
print("AB\nC\nDE")
```

    AB
    C
    DE
    

#### 2/


```python
"heyPhan".find("Phan")
```




    3



#### 3/ 

Name = "Kevin Phan"
Name[-1] would be?
-> Answer: n

#### 4/


```python
A = "python basics kevinph4n"
B = A.title()
print(B)
```

    Python Basics Kevinph4N
    
