# 🐍 Python OOP: Abstract Class & Method Example

## 🎯 AIM

To create an **abstract class** named `Shape` with an **abstract method** `calculate_area`, and implement this method in two subclasses: `Rectangle` and `Circle`.

---

## 🧠 ALGORITHM

1. **Import ABC module**:
   - Use `from abc import ABC, abstractmethod` to define abstract classes and methods.

2. **Create Abstract Class `Shape`**:
   - Define an abstract method `calculate_area()` with `@abstractmethod`.

3. **Create Subclass `Rectangle`**:
   - Set default values for `length` and `breadth`.
   - Override `calculate_area()` to compute the rectangle area.

4. **Create Subclass `Circle`**:
   - Set default value for `radius`.
   - Override `calculate_area()` to compute the circle area.

5. **Create Objects & Call Methods**:
   - Instantiate `Rectangle` and `Circle`.
   - Call their `calculate_area()` methods.

---

## 💻 Program
```
import math
from abc import ABC, abstractmethod
class Shape(ABC):
   def __init__(self,l,b,r):
      self.r=r
      self.l=l
      self.b=b
   @abstractmethod
   def calculate_area(self):
      pass
class Rectangle(Shape):
   def calculate_area(self):
      return self.l*self.b
class Circle(Shape):
   def calculate_area(self):
      return self.r*self.r*math.pi
obj=Rectangle(10,20,15)
print(f"Area of the Rectangle : {obj.calculate_area()}")
obj=Circle(10,20,15)
print(f"Area of the Circle : {obj.calculate_area():.2f}")
```
## Output
![alt text](<Screenshot (64).png>)
## Result
The following python program is executted successfully.
