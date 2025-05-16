# Python Program to Define an Abstract Base Class for Polygon and Implement Its Subclasses

# Aim
To create an abstract base class `Polygon` with an abstract method `sides()` and implement it in various subclasses that represent different shapes (e.g., Triangle, Square). Each subclass will define its own version of the `sides()` method.

# Procedure
1. Define an abstract base class `Polygon` using the `ABC` module and the `@abstractmethod` decorator.
2. In the `Polygon` class, define an abstract method `sides()`.
3. Create subclasses like `Triangle` and `Square` that inherit from `Polygon` and implement the `sides()` method.
4. Create objects of these subclasses and call the `sides()` method.
# Program
```python
from abc import ABC,abstractmethod
  
class Polygon(ABC):   
  
   # abstract method   
   def sides(self):   
      pass  
  
class Triangle(Polygon):   
  
     
   def sides(self):   
      print("Triangle has 3 sides")   
  
class Pentagon(Polygon): 
    def sides(self):
        print("Pentagon has 5 sides")
  
     
   #Add code here
class Hexagon(Polygon): 
    def sides(self):
        print("Hexagon has 6 sides")
  
   #Add your code
class square(Polygon):   
  
   def sides(self):   
      print("I have 4 sides")   
  
# Driver code   
t = Triangle() 
t.sides()
  
s = square()   
s.sides()
  
p = Pentagon()   
p.sides() 
  
k = Hexagon()   
k.sides()
```

# Output

![image](https://github.com/user-attachments/assets/e9341ea0-6d0a-4da5-81e1-cc610f5d08d8)

# Result
The program successfully defines the abstract class and implements it in subclasses. When the `sides()` method is invoked, it returns the number of sides of the respective polygons.

