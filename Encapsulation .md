# 🐍 Python OOP: Encapsulation with Private Members

## 🎯 AIM

To implement **Encapsulation** in Python by defining a class `Rectangle` with **private member variables** `__length` and `__breadth`.

---

## 🧠 ALGORITHM

1. **Define the Class**:
   - Create a class `Rectangle` with two private attributes: `__length` and `__breadth`.

2. **Initialize Variables**:
   - Use the `__init__()` constructor to set initial values for `__length` and `__breadth`.

3. **Print Values**:
   - Display the private variables from within the class to demonstrate access.

4. **Instantiate the Object**:
   - Create an object of the `Rectangle` class to trigger the constructor.

---

## 💻 Program
```
   class Rectangle():
      def __init__(self,l,b):
         self.__l=l
         self.__b=b
      def display(self):
         print(f"Length : {self.__l}\nBreath : {self.__b}")
   obj=Rectangle(10,20)
   obj.display()
```
## Output
![alt text](<Screenshot (65).png>)
## Result
The following python program is executted successfully.
