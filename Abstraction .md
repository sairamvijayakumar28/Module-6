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
class shape(ABC):
    @abstractmethod
    def calculate_area(self):
        pass

class Rectangle(shape):
    length = 6
    breadth = 4
    def calculate_area(self):
        return self.length * self.breadth

class Circle(shape):
    radius = 7
    def calculate_area(self):
        return 3.14*self.radius**2

r = Rectangle()
c = Circle() 

print("Area of a rectangle:", r.calculate_area())
print("Area of a circle:", c.calculate_area()) 

```
## Output
<img width="485" height="179" alt="image" src="https://github.com/user-attachments/assets/80b74b27-f889-43d5-a029-a4da653d8d37" />

## Result
Thus,the above python program executed succesfully.
