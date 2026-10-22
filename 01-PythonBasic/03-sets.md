### Sets
- unlike lists and tuples, sets are unordered (do not record element position)


```python
music_genres_1 = {'ballad', 'bop', 'rock', 'bop', 'RnB', 'disco'}
print(music_genres_1)
# -> duplicate items will not be present in Sets
```

    {'ballad', 'disco', 'rock', 'bop', 'RnB'}
    

#### 1/ .set()


```python
list1 = ['kevinph4n', 'is', 'handsome', 'handsome', 2008]
list1_set = set(list1)
print(list1_set)
```

    {'is', 'kevinph4n', 'handsome', 2008}
    

#### 2/ .add()


```python
A = {"thriller", "ballad", "rnb"}
A.add("kevin")
print(A)
```

    {'rnb', 'kevin', 'thriller', 'ballad'}
    


```python
A = {"thriller", "ballad", "rnb"}
A.add("kevin")
"kevin" in A
```




    True



#### 3/ Sets Mathematical Set Operations


```python
# &
album_set1 = {"X", "French Exit", "HVL"}
album_set2 = {"X", "French Exit", "Loi Choi"}
album_set_similar = album_set1 & album_set2
print(album_set_similar)
```

    {'X', 'French Exit'}
    


```python
# .union()
album_set1 = {"X", "French Exit", "HVL"}
album_set2 = {"X", "French Exit", "Loi Choi"}
album_set_union = album_set1.union(album_set2)
print(album_set_union)
```

    {'X', 'Loi Choi', 'HVL', 'French Exit'}
    


```python
# .issubset()
album_set1 = {"X", "French Exit"}
album_set2 = {"X", "French Exit", "HVL"}
album_set1.issubset(album_set2)
```




    True


