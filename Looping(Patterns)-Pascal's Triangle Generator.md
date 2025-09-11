# 🔺 Looping(Patterns)-Pascal's Triangle Generator in Python

This project demonstrates a simple Python program to generate **Pascal’s Triangle**, where the number of rows is provided by the user.

---

## 🎯 Aim

To write a Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user.

---

## 🧠 Algorithm

1. Start the program.
2. Input the number of rows from the user.
3. Loop from 0 to the number of rows.
4. For each row:
   - Print appropriate spaces to shape the triangle.
   - Compute values using the formula:  
     \[
     C(n, k) = \frac{n!}{k!(n-k)!}
     \]
5. Print all rows of Pascal’s Triangle.
6. End the program.

---

## 🧪 Program
```
def generate_pascals_triangle(rows):
    triangle = []
    for i in range(rows):
        row=[1]*(i+1)
        for j in range(1,i):
                 row[j]=triangle[i-1][j-1]+triangle[i-1][j]
        triangle.append(row)
    return triangle
def print_pascal_triangle(triangle):
    for row in triangle:
        print(' '.join(map(str,row)))
num_rows=int(input())

pascal_triangle=generate_pascals_triangle(num_rows)
print_pascal_triangle(pascal_triangle)
```

## Sample Output
<img width="559" height="536" alt="image" src="https://github.com/user-attachments/assets/9e49a3ab-4253-42f1-8e50-dbd7f5a4d85e" />


## Result
Thus,a Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user is created successfully.

