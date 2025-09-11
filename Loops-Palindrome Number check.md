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
