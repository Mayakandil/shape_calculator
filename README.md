# Shape Area Calculator 📐

This Python program calculates the area of different shapes using a single function `CalcArea()`.  
It supports triangles, rectangles, squares, and circles.  
If an unsupported shape is entered, the function returns `"invalid shape"`.

---

## 🔧 Code Used

```python
import math

def CalcArea(shape, a, b=0):
    shape = shape.lower()

    if shape == "triangle":
        area = 0.5 * a * b
    elif shape == "rectangle":
        area = a * b
    elif shape == "circle":
        area = math.pi * (a ** 2)
    elif shape == "square":
        area = a * a
    else:
        return "invalid shape"

    return area

print("Triangle:", CalcArea('triangle', 10, 7))
print("Rectangle:", CalcArea('rectangle', 10, 7))
print("Square:", CalcArea('square', 5))
print("Circle:", CalcArea('circle', 10))
print(CalcArea("hexagon", 5))



# 📌How It Works
- The function CalcArea() takes:
    - shape → the name of the shape
    - a → main dimension
    - b → optional second dimension (default = 0)
- Supported shapes:
    - triangle → 0.5 × a × b
    - rectangle → a × b
    - circle → π × a²
    - square → a × a
- If the shape is not recognized, the function returns:
   -> "invalid shape"


# 🧪 Example Output
->
   Triangle: 35.0
   Rectangle: 70
   Square: 25
   Circle: 314.1592653589793
   invalid shape


# 🚀 How to Run
- Make sure Python 3.x is installed.
- Save the script as:
         area_calculator.py
- Run the program:
         python area_calculator.py



# 📚 Features
- Calculates area of multiple shapes.
- Uses a single unified function.
- Automatically rejects invalid shapes.
- Clean and beginner-friendly implementation.
- Uses Python's math module for circle calculations.


# 🔮 Possible Improvements
- Ask the user for input instead of fixed values.
- Add more shapes (hexagon, pentagon, ellipse, etc.).
- Add error-handling for non-numeric values.
- Build a GUI version using Tkinter.
- Convert the function into a class-based design.
