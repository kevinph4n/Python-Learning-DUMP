## **Exercise 1: Create a 1D NumPy array of numbers from 0 to 9**
**Expected Output:**
`[0 1 2 3 4 5 6 7 8 9]`


```python
import numpy as np
array = np.arange(10)
print(array)
```

    [0 1 2 3 4 5 6 7 8 9]
    

---
## **Exercise 2: Convert 1D array to 2D**
**Given:**
```
import numpy as np
arr = np.arange(6)
```
**Expected Output:**
```
Original Array: [0 1 2 3 4 5]
Reshaped 2x3 Array:
 [[0 1 2]
 [3 4 5]]



```python
import numpy as np

array = np.arange(6)
array_2d = array.reshape(2, 3)
print('Original Array:', array)
print('Reshaped 2x3 Array:\n', array_2d)
```

    Original Array: [0 1 2 3 4 5]
    Reshaped 2x3 Array:
     [[0 1 2]
     [3 4 5]]
    

---
## **Exercise 3: Print Array Attributes**

**Instructions**: Print the following attributes of the array:
```
The shape of the array.
The number of array dimensions.
The size of each element in bytes.
```
**Given**:
```
import numpy as np
my_array = np.array([[1, 2], [3, 4], [5, 6], [7, 8]], dtype=np.uint16)
```
**Expected Output**:
```
The shape of the array is: (4, 2)
The number of dimensions is: 2
The size of each element in bytes is: 2



```python
import numpy as np

my_array = np.array([[1,2], [3,4], [5,6], [7,8]], dtype = np.uint16)
# Create the 4x2 array of type unsigned int16
# We use np.array() and specify the dtype

# Print the attributes
print("The shape of the array is:", my_array.shape)
print("The number of dimensions is:", my_array.ndim)
print("The size of each element in bytes is:", my_array.itemsize)
```

    The shape of the array is: (4, 2)
    The number of dimensions is: 2
    The size of each element in bytes is: 2
    
