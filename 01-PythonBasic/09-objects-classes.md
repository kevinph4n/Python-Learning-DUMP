- every object has **a type, an internal data representation (a blueprint), a set of procedures for interacting with the object (method)**
- An object is an **instance** of a particular **type**
-e.g Type 1: Object 1, Object 2,...

### Objects
#### 1/ Types:
- using type() to find **the type of an object**


```python
type(1)
```




    int




```python
type('kevin')
```




    str



#### 2/ Methods:
- for example: **.sort(), .append(), .add()**

---
### Classes
#### 1/ Defining classes
- Class includes both **Data attributes & Methods**
- You can create classes, for examples:


##### 1.1/ Class Car
-> **Data attributes**: brand, color


```python
class Car: # define your class

    def __init__(self, brand, color): # self is self parameter
        # brand and color are parameters
        self.brand = brand
        self.color = color
# those are data attributes used to initialize each instance of the class
```

#### 2/ Create an instance of a Class: Car


```python
class Car(object): #(object) is optional, in Python 2 we don't need (object)
    def __init__(self, brand, color): 
        self.brand = brand
        self.color = color
    def drive(self):
        print(f"The {self.color} {self.brand} is driving")

VinFast = Car('VinFast', 'red') 

VinFast.drive()

```

    The red VinFast is driving
    


```python
# NO __init__
class ToanTinTCTA:
    pass
    # this class is completely empty, no automatically assign a value or anything

# So now, if we want to create 2 individuals:
person1 = ToanTinTCTA()
person2 = ToanTinTCTA()
# U have to manually assign values to them, cuz its not automatic
person1.name = "Hong Phuc"
person1.username = "kevinph4n"

person2.name = "Hung Dan"
person2.username = "hungdan"

print(person1.name)
```

    Hong Phuc
    


```python
# WITH __init__
class ToanTinTCTA:
    def __init__(self, name, username):
        self.name = name
        self.username = username

person1 = ToanTinTCTA("Hong Phuc", "kevinph4n")
person2 = ToanTinTCTA("Hung Dan", "hungdan")

print(person1.name)
```

    Hong Phuc
    

### More examples


```python
# Class
class WorldCup:
    pass
```


```python
# Object
class WorldCup:
    pass
Messi = WorldCup()
```


```python
# Variables bound to an object
class WorldCup_0:
    def __init__(self, full_name, won_the_wc, has_a_wife):
        self.full_name = full_name
        self.won_the_wc = won_the_wc
        self.has_a_wife = has_a_wife
messi = WorldCup_0("Lionel Messi", "Yes", "1 Wife")
print(messi.full_name)
print(messi.won_the_wc)
print(messi.has_a_wife)



```

    Lionel Messi
    Yes
    1 Wife
    


```python
class WorldCup_1:
    def trash_talk(self):# Method
        print("I have money!")

messi = Fighter()
messi.trash_talk()
```

    I'm the best!
    


```python
# Inheritance: Child class inherits from parent class

class Athlete:
    pass

class Fighter(Athlete):# Inheritance 
    pass
```


```python
# Example using inheritance 

class WorldCup_2:

  def height(self, height):
      # Maps height to height class
      return "Short"  

# Footballer class inherits from WorldCup_2
class Footballer(WorldCup_2):

  def __init__(self, name):
    self.name = name
  
  def print_name(self):
    print(self.name)

footballer = Footballer("Messi")  
print(footballer.height(160)) 
footballer.print_name()
```

    Short
    Messi
    


```python
class student:
    def __init__ (self, name, age, GPA):
        self.GPA = GPA
        self.name = name
        self.age = age

HungDan = student("Hung Dan", 21, 4.0)
HongPhuc = student("Hong Phuc", 18, 4.0)

print("HongPhuc's age: ", HongPhuc.age)
print("HungDan's GPA: ", HungDan.GPA)
```

    HongPhuc's age:  18
    HungDan's GPA:  4.0
    


```python

```
