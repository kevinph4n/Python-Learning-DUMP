### **Exercise 1. Arithmetic Product and Conditional Logic**
**Practice Problem 1:** Write a Python function that accepts two integer numbers. If the product of the two numbers is less than or equal to 1000, return their product; otherwise, return their sum.

**Exercise Purpose:** Learn basic control flow and the use of if-else statements. Understand how code decisions change output based on a mathematical threshold.

**Given Input:**
Case 1: number1 = 20, number2 = 30
Case 2: number1 = 40, number2 = 30

**Expected Output:**
```
The result is 600
The result is 70
```

**Solution:**

```python
# Exercise 1. Arithmetic Product and Conditional Logic

def product_of_2_numbers(number1, number2):
    product = number1 * number2
    if product <= 1000:
        return product
    else:
        return number1 + number2
# Case 1:
result = product_of_2_numbers(20,30)
print("The result is", result)
# Case 2:
result = product_of_2_numbers(40,30)
print("The result is", result)


```

    The result is 600
    The result is 70
    

---

### **Exercise 2. Cumulative Sum of a Range**
**Practice Problem:** Iterate through the first 10 numbers (0–9). In each iteration, print the current number, the previous number, and their sum.

**Exercise Purpose:** This exercise teaches “State Tracking.” In programming, you often need to remember a value from a previous loop iteration to calculate results in the current one. This is the basis for algorithms like Fibonacci sequences or running totals.

**Given Input:** Range: numbers = range(10)

**Expected Output:**
```
Printing current and previous number sum in a range(10)
Current Number 0 Previous Number 0 Sum: 0
Current Number 1 Previous Number 0 Sum: 1
Current Number 2 Previous Number 1 Sum: 3
....
Current Number 8 Previous Number 7 Sum: 15
Current Number 9 Previous Number 8 Sum: 17
```

**Solution:**

```python
print("Printing current and previous number sum in a range(10)")
previous_num = 0

# Loop from 0 to 9
for i in range(10):
    x_sum = previous_num + i
    print(f"Current Number {i} Previous Number {previous_num} Sum: {x_sum}")
    
    # Update previous_num for the next iteration
    previous_num = i
#Initialization: previous_num = 0 is set outside the loop so it persists across iterations.
# for loop Iteration: The for i in range(10) loop automatically increments i from 0 to 9.
# Next, display the current number (i), the previous number, and the addition of both numbers in each iteration of the loop.
# State Update: The line previous_num = i is critical; it “shifts” the current value into the “memory” slot for the next cycle of the loop.
```

```
    Printing current and previous number sum in a range(10)
    Current Number 0 Previous Number 0 Sum: 0
    Current Number 1 Previous Number 0 Sum: 1
    Current Number 2 Previous Number 1 Sum: 3
    Current Number 3 Previous Number 2 Sum: 5
    Current Number 4 Previous Number 3 Sum: 7
    Current Number 5 Previous Number 4 Sum: 9
    Current Number 6 Previous Number 5 Sum: 11
    Current Number 7 Previous Number 6 Sum: 13
    Current Number 8 Previous Number 7 Sum: 15
    Current Number 9 Previous Number 8 Sum: 17
```

---
### **Exercise 3. String Indexing and Even Slicing**

**Practice Problem**: Display only those characters which are present at an even index number in given string.

**Exercise Purpose**: Understand how data is stored in memory using zero-based indexing. In most languages, the first character is at position 0, the second at 1, and so on. Mastering indexing is vital for data parsing.

**Given Input**: String: "pynative"

**Expected Output**:
```
Original String is  pynative
Printing only even index chars
p
n
t
v
```

**Solution:**

```python
String = "pynative"
print('Original String is', String)
even_index_chars = String[0::2]

print("Printing only even index chars ")
for chars in even_index_chars:
    print(chars)
```
```
    Original String is pynative
    Printing only even index chars 
    p
    n
    t
    v
```

---
## **Exercise 4. String Slicing and Substring Removal**
**Practice Problem**: Write a function to remove characters from a string starting from index 0 up to n and return a new string.

**Exercise Purpose**: This exercise demonstrates how to truncate data strings, a common data-cleaning task.

**Given Input**:
```
remove_chars("pynative", 4)
remove_chars("pynative", 2)
```
**Expected Output**:
```
tive
native
```

**Solution:**


```python
def remove_chars(word, n):
    print('Original string:', word)
    # Extract string from index n to the end
    res = word[n:]
    return res

print("Removing characters from a string")
print(remove_chars("pynative", 4))
print(remove_chars("pynative", 2))
```
```
    Removing characters from a string
    Original string: pynative
    tive
    Original string: pynative
    native
```

---
## **Exercise 5. Variable Swapping (The In-Place Method)**

**Practice Problem**: Write a program to swap the values of two variables, a and b, without using a third temporary variable.

**Exercise Purpose**: This exercise will help you learn about memory efficiency and Python’s special tuple unpacking feature. In other languages like C or Java, you need a temporary variable to swap values safely. In Python, you can swap values in one line without risking data loss.

**Given Input**: a = 5, b = 10

**Expected Output**:
```
Before Swap: a = 5, b = 10
After Swap: a = 10, b = 5
```

**Solution:**

```python
a =5
b=10
print(f"Before Swap: a = {a}, b = {b}")

a, b = b, a
print(f"After Swap: a = {a}, b = {b}")
```
```
    Before Swap: a = 5, b = 10
    After Swap: a = 10, b = 5
```

---
## **Exercise 6. Calculating Factorial with a Loop**

**Practice Problem**: Write a program that calculates the factorial of a given number (e.g., 5!) using a for loop.

**Exercise Purpose**: This exercise explores “Mathematical Accumulation.” A factorial (e.g., 5! = 5*4*3*2*1) requires you to maintain a running product across multiple iterations, which is a core pattern in scientific computing.

**Given Input**: `number = 5`

**Expected Output**: `The factorial of 5 is 120`

**Solution:**


```python
num = 5
factorial = 1

# Loop from 1 to num (inclusive)
for i in range(1, num + 1):
    factorial = factorial * i

print(f"The factorial of {num} is {factorial}")
# Identity Element: We start factorial at 1 because multiplying by zero would ruin the entire calculation.
# range(1, num + 1): Since the end of a range is exclusive, we use + 1 to ensure the loop includes the number 5.
# Running Product: Each pass of the loop updates the value of factorial, building the final result step-by-step.
```

``The factorial of 5 is 120``

---
## **Exercise 7. List Manipulation: Add and Remove**

**Practice Problem**: Create a list of 5 fruits. Add a new fruit to the end of the list, then remove the second fruit (at index 1).

**Exercise Purpose**: This exercise teaches “Dynamic Collection Management.” Lists are rarely static; being able to modify, expand, and prune them is essential for handling data like shopping carts, user lists, or inventory systems.

**Given Input**: `fruits = ["apple", "banana", "cherry", "date", "elderberry"]`

**Expected Output**: `['apple', 'cherry', 'date', 'elderberry', 'fig']`

**Solution:**

```python
fruits = ['apple', 'banana', 'cherry', 'date', 'elderberry']
fruits.pop(1)
fruits.append('fig')
print(fruits)
```

``['apple', 'cherry', 'date', 'elderberry', 'fig']``
    

---
## **Exercise 8. String Reversal**

**Practice Problem**: Write a program that takes a string and reverses it (e.g., “Python” becomes “nohtyP”).

**Exercise Purpose**: This exercise demonstrates “Sequence Slicing.” Strings in Python are sequences, and mastering the slicing syntax is a powerful shortcut for data manipulation that would take 5-10 lines of code in other languages.

**Given Input**: ``text = "Python"``

**Expected Output**: ``Reversed: nohtyP``

**Solution:**

```python
text = "Python"
reversedtext = text[::-1] # [start:end:step]
# The first two colons imply “start at the very beginning” and “go to the very end.”
# The -1 indicates the direction of travel.
print("text =", text)
print("Reversed:", reversedtext)

```
```
    text = Python
    Reversed: nohtyP
```

---
## **Exercise 9. Vowel Frequency Counter**

**Practice Problem**: Write a program to count the total number of vowels (a, e, i, o, u) present in a given sentence.

**Exercise Purpose**: This exercise introduces “Membership Testing.” By checking if a character belongs to a specific group (the vowels), you learn how to filter data based on categories. This is a fundamental step toward building text-analysis tools or spam filters.

**Given Input**: `sentence = "Learning Python is fun!"`

**Expected Output**: `Number of vowels: 6`

**Solution:**

```python
sentence = "Learning Python is fun!"
vowels = "aeiou" # define a string containing all vowels "aeiou" 
count = 0

# Convert to lowercase to handle 'A' and 'a' equally
for char in sentence.lower():
    if char in vowels:
        count += 1

print(f"Number of vowels: {count}")
# .lower(): This is essential for robust code. It ensures that “A” and “a” are both counted
# The 'in' Keyword: a highly optimized Python operator that checks for the existence of an item within a sequence (the string of vowels).
# Counter Pattern: We use a simple integer (count) that “accumulates” every time the condition evaluates to True.

```

``Number of vowels: 6``
    
---
## **Exercise 10. Finding Extremes (Min/Max) in a List**

**Practice Problem**: Given a list of integers, find and print both the largest and the smallest numbers.

**Exercise Purpose:** This exercise explores “Aggregate Functions.” While Python has built-in tools for this, understanding how to identify extremes is critical for data normalization, where you often need to find the range of a dataset before processing it.


**Given Input**: ``nums = [45, 2, 89, 12, 7]``

**Expected Output**: ``Largest: 89 Smallest: 2``

**Solution:**

```python
nums = [45, 2, 89, 12, 7]

largest = max(nums)
smallest = min(nums)

print(f"Largest: {largest}")
print(f"Smallest: {smallest}")
# max(nums): Internally, this function assumes the first element is the largest, then compares it against every other element in the list, updating the “current winner” as it goes.
# min(nums): Works identically to max, but tracks the lowest value found.
# Algorithm Efficiency: These functions only need to pass through the list once, making them very fast even for lists with millions of items.

```
```
    Largest: 89
    Smallest: 2
```
---
## **Exercise 11. Removing Duplicates from a List**

**Practice Problem**: Write a script that takes a list containing duplicate items and returns a new list with only unique elements.

**Exercise Purpose:** This exercise teaches “Data De-duplication.” In real-world data science, datasets are often “messy” with repeating entries. Mastering the conversion between Lists (which allow duplicates) and Sets (which do not) is the fastest way to clean data.


**Given Input**: ``data = [1, 2, 2, 3, 4, 4, 4, 5]``

**Expected Output**: ``Unique List: [1, 2, 3, 4, 5]``

**Solution:**

```python
data = [1, 2, 2, 3, 4, 4, 4, 5]

# Set conversion removes duplicates automatically
unique_data = list(set(data))

print(f"Unique List: {unique_data}")

```

``Unique List: [1, 2, 3, 4, 5]``

---
## **Exercise 12. List Comparison and Boolean Logic**

**Practice Problem:** Write a function to return True if the first and last number of a given list is the same. If the numbers are different, return False.

**Exercise Purpose:** This exercise introduces “Collection Indexing” and “Boolean Flags.” Comparing data structure boundaries is common in pattern matching and data integrity checks.

**Given Input:**
```
numbers_x = [10, 20, 30, 40, 10]
numbers_y = [75, 65, 35, 75, 30]
```

**Expected Output:**
```
Given list: [75, 65, 35, 75, 30] | result is False
Given list: [10, 20, 30, 40, 10] | result is True
```
**Solution:**

```py
def first_last_same(number_list):
    print("Given list:", number_list)
    
    first_num = number_list[0]
    last_num = number_list[-1]
    
    if first_num == last_num:
        return True
    else:
        return False

numbers_x = [10, 20, 30, 40, 10]
print("result is", first_last_same(numbers_x))

numbers_y = [75, 65, 35, 75, 30]
print("result is", first_last_same(numbers_y))
# Negative Indexing: Python allows [-1] to represent the last item in a list regardless of the list’s length. This is safer and cleaner than calculating len(list) - 1.
# Equality Operator (==): This operator compares the values of the two objects and evaluates to a Boolean (True/False).
# Logic Gate: The function provides a clear binary answer based on the structural properties of the input list.
```
```
Given list: [10, 20, 30, 40, 10]
result is True
Given list: [75, 65, 35, 75, 30]
result is False
```
---
## **Exercise 13. Filtering Lists with Conditional Logic**

**Practice Problem:** Iterate through a given list of numbers and print only those numbers which are divisible by 5.

**Exercise Purpose:** This exercise teaches the use of the modulo operator (%) and loop filtering. In data processing, you often need to sift through large datasets to extract subsets that meet mathematical criteria.

**Given Input:** ``num_list = [10, 20, 33, 46, 55]``

**Expected Output:**
```
Divisible by 5:
10, 20, 55
```
**Solution:**

```py
num_list = [10, 20, 33, 46, 55]
print("Given list is", num_list)
print("Divisible by 5:")

# Iterate through each element
for num in num_list:
    # Check divisibility
    if num % 5 == 0:
        print(num)

# for num in num_list: This construct allows the program to visit every item in the collection without needing to track indices manually.
# num % 5 == 0: The modulo operator returns the remainder. If the remainder of division by 5 is 0, the number is a multiple of 5.
# Filtering Logic: Only when the if condition evaluates to True does the print function execute, effectively “filtering” the list.
```
```
Given list is [10, 20, 33, 46, 55]
Divisible by 5:
10
20
55
```
---
## **Exercise 14. Substring Frequency Analysis**

**Practice Problem:** Write a program to find how many times the substring “Emma” appears in a given string.

**Exercise Purpose:** Text analysis and pattern matching are core pillars of programming. This exercise introduces searching for a “needle in a haystack,” a fundamental concept for building search engines or data validation tools.

**Given Input:**
```
str_x = "Emma is good developer. Emma is a writer"
Expected Output: Emma appeared 2 times
```

**Solution:**

```py
str_x = "Emma is good developer. Emma is a writer"
count = str_x.count("Emma")
print(f"Emma appeared {count} times")
```
``Emma appeared 2 times``

---
## **Exercise 15. Nested Loops for Pattern Generation**

**Practice Problem:** Print the following pattern where each row contains a number repeated a specific number of times based on its value.

**Exercise Purpose:** Pattern printing is a classic way to learn “Nested Loops.” You coordinate an outer loop for rows and an inner loop for columns or repetitions. This improves spatial logic and control over output formatting.

**Given Input:** Range: 1 to 5

**Expected Output:** 
```
1 
2 2 
3 3 3 
4 4 4 4 
5 5 5 5 5
```

**Solution:**

```py
# Outer loop for rows
for num in range(1, 6):
    # Inner loop for repetition
    for i in range(num):
        print(num, end=" ") # end=" " keeps it on the same line
    # New line after each row
    print("\n")
# Nested Loops: The outer loop num sets the “context” for the row. The inner loop i performs the work for that specific row.
# end=" ": By default, print() adds a newline. Overriding this with a space allows multiple numbers to appear side-by-side.
# Formatting: The final print("\n") acts as a “carriage return,” starting the next row of the pattern on a clean line.
```
```
1 
2 2 
3 3 3 
4 4 4 4 
5 5 5 5 5
```








