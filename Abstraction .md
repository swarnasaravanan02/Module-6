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
from abc import ABC, abstractmethod

import math

class Shape(ABC):

    @abstractmethod
    
    def calculate_area(self):
    
        pass
    
class Rectangle(Shape):

    length = 5
    breadth =3 
    def calculate_area(self):
        return self.length * self.breadth

class Circle(Shape):

  radius = 4
  
  def calculate_area(self):
  
      return 3.14 * self.radius * self.radius

rec = Rectangle()

cir = Circle()

print("Area of a rectangle:", rec.calculate_area()) #call to 'calculate_area' method defined inside the class 'Rectangle'

print("Area of a circle:", cir.calculate_area()) #call to 'calculate_area' method defined inside the class 'Circle'.
```
## Output
<img width="607" height="182" alt="image" src="https://github.com/user-attachments/assets/8fdd9cae-4afd-4dfe-b40a-1105dbf5fe79" />

## Result
Thus, the program to implement Abstract Class & Method in Python was executed successfully and produced the expected result.
