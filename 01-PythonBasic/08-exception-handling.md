### Expception Handling

#### 1/ try...except...else...finally statements


```python
try:
    openApplication = open('myApplication', 'r')
    openApplication.write('My application for this lesson')

except Error():
    print('Unable to open the application')

else:
    print('I dont even know at this point')

finally:
    openApplication.close()
    print('Application closed')

```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    Cell In[8], line 1
    ----> 1 myApplication()
          2 try:
          3     openApplication = open('myApplication', 'r')
          4     openApplication.write('My application for this lesson')
    

    NameError: name 'myApplication' is not defined



```python
# using Try- except. Attempting to divide by Zero
try:
    # Attempting to divide 10 by 0
    result = 10 / 0
except ZeroDivisionError:
    # Handling the ZeroDivisionError and printing an error message
    print("Error: Cannot divide by zero")
# This line will be executed regardless of whether an exception occurred
print("outside of try and except block")
```

    Error: Cannot divide by zero
    outside of try and except block
    
