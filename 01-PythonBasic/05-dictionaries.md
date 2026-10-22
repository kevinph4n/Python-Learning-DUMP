```python
dict = {"kevin": 2008, "kate": 2007 , "nvi": 2006 }
# so the Thriller,... is the key
# the 1980, 1982,... is the value
"kevin" in dict
```




    True



#### 1/ .values()


```python
dict = {"kevin": 2008, "kate": 2007 , "nvi": 2006 }
dict.values()
```




    dict_values([2008, 2007, 2006])



#### 2/ .keys()


```python
dict = {"kevin": 2008, "kate": 2007 , "nvi": 2006 }
dict.keys()
```




    dict_keys(['kevin', 'kate', 'nvi'])




```python
dict = {"D":(4,4,4)}
dict["D"]
```




    (4, 4, 4)




```python
dict = {"kevin": 2008, "kate": 2007 , "nvi": 2006 }
list(dict.keys())
```




    ['kevin', 'kate', 'nvi']


