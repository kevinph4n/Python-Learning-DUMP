### File object


```python
# Read the content
with open('D:/text1.txt', 'r') as file:
    file_stuff = file.read()
    print(file_stuff)
```

    aaaaaa
    


```python
# Write the content
with open('D:/text1.txt', 'w') as file1:
    file1.write("this is kevin \n kevinph4n")

```


```python
# Write multiples lines using list and loop
lines = ['Line 1', ' Line 2', 'Line 3']

with open('D:/text1.txt', 'w') as file1:
    for line in lines:
        file1.write(line + '\n')

# -> Output in the file: Line 1 \n Line 2 \n Line 3
```
