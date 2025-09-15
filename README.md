# Built-in Functions -Binary Conversion Using Built-in Functions in Python

## 🎯 Aim
To write a Python program to convert the number **76** into its **binary representation** using built-in Python functions.

## 🧠 Algorithm
1. Assign the value `76` to a variable `a`.
2. Use the built-in `bin()` function to convert the number to binary.
3. Print the result.

## 🧾 Program
```
decimal_number=76
binary_number=bin(decimal_number)
print(binary_number)
```

## Output
<img width="282" height="87" alt="Screenshot 2025-09-11 201517" src="https://github.com/user-attachments/assets/433d3be2-b07e-44ab-bfde-d713bda5f2cf" />


## Result
Thus,the Python program to convert the number **76** into its **binary representation** using built-in Python functions is created successfully.


# Functions in Python: Modulo Calculator

## 🎯 Aim
To write a Python program that defines a function which accepts two values and returns their **modulo** using the `%` operator.

## 🧠 Algorithm
1. Define a function called `result` that takes two arguments `a` and `b`.
2. Inside the function, compute the modulo using `a % b`.
3. Print the result of the modulo operation.
4. Get two integer inputs from the user.
5. Call the `result` function with the user-provided values.

## 🧾 Program
```
def result(a,b):
    result=a%b
    return result
a=int(input())
b=int(input())
modulo_result=result(a,b)
print(f"modulo is {modulo_result}")
```

## Output
<img width="572" height="246" alt="Screenshot 2025-09-11 202409" src="https://github.com/user-attachments/assets/6bdca1b6-1c99-4309-8cf9-667812210c53" />


## Result
Thus, a Python program that defines a function which accepts two values and returns their **modulo** using the `%` operator is created successfully.


# Lambda Function in Python: Addition of Two Numbers

## 🎯 Aim
To write a Python program that defines a **lambda function** which takes two arguments `a` and `b`, and returns their sum.

## 🧠 Algorithm
1. Get two integer inputs from the user.
2. Use a **lambda function** to define a function `f` that returns `a + b`.
3. Call the function with the user inputs and print the result.

## 🧾 Program
```
def add(a, b):
    return a + b

f = add

a = int(input())
b = int(input())
result = f(a, b)
print(result)
```

## Output
<img width="427" height="251" alt="Screenshot 2025-09-11 202724" src="https://github.com/user-attachments/assets/d1b1bcae-3a63-4608-8cd1-c85cd8e80313" />


## Result
Thus, a Python program that defines a **lambda function** which takes two arguments `a` and `b`, and returns their sum is created successfully.


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

## Loops in Python: Palindrome Number Checker

## 🎯 Aim
To write a Python program that checks whether a given number is a **palindrome** using loops.

## 🧠 Algorithm
1. Get input from the user and assign it to a variable `num`.
2. Assign the value of `num` to a temporary variable `temp`.
3. Initialize a variable `rev` to 0 (used to store the reversed number).
4. Use a `while` loop to reverse the digits:
   - While `temp > 0`:
     - `rev = (10 * rev) + temp % 10`
     - `temp = temp // 10`
5. After the loop, compare `rev` with `num`:
   - If equal, print that the number is a palindrome.
   - Else, print that it is not a palindrome.

## 🧾 Program
```
def is_palindrome(num):
    num_str=str(num)
    reversed_str=num_str[::-1]
    
    if num_str==reversed_str:
        return True
    else:
        return False
            
input_number=int(input())
if is_palindrome(input_number):
    print(f"The given number {input_number} is a Palindrome")
else:
    print(f"The given number {input_number} is not a palindrome")
```
## Output
<img width="1033" height="196" alt="image" src="https://github.com/user-attachments/assets/f0fbb62f-6bc8-4798-b260-b6bd1240dbe0" />



## Result
Thus,a Python program that checks whether a given number is a **palindrome** using loops is created successfully.

