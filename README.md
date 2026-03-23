# Built-in Functions -Binary Conversion Using Built-in Functions in Python

## 🎯 Aim
To write a Python program to convert the number **16** into its **binary representation** using built-in Python functions.

## 🧠 Algorithm
1. Assign the value `16` to a variable `a`.
2. Use the built-in `bin()` function to convert the number to binary.
3. Print the result.

## 🧾 Program
```
a=16 

print(bin(a)
```
## Output
<img width="562" height="265" alt="image" src="https://github.com/user-attachments/assets/d42d2a9e-78ec-45e8-bd51-4f797265cd12" />

## Result
Thus, the program has been successfully executed.

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
def result(a, b):
    modulo_value = a % b
    return modulo_value

a=int(input())
b=int(input())
print("modulo is", result(a, b))
```
## Output
<img width="662" height="311" alt="image" src="https://github.com/user-attachments/assets/209fd2e2-b101-4b38-a285-8e30d3f4dacd" />

## Result
Thus,The program to return two values modulo is successful.

# Lambda Function in Python: Addition of Two Numbers

## 🎯 Aim
To write a Python program that defines a **lambda function** which takes two arguments `a` and `b`, and returns their sum.

## 🧠 Algorithm
1. Get two integer inputs from the user.
2. Use a **lambda function** to define a function `f` that returns `a + b`.
3. Call the function with the user inputs and print the result.

## 🧾 Program
```
a=int(input()) 

b=int(input()) 

f=lambda a,b: a+b 

print(f(a,b))
```

## Output
<img width="325" height="249" alt="image" src="https://github.com/user-attachments/assets/19a96b50-e99b-4b4c-9fe7-979bd63e30e2" />

## Result
Thus, the program has been successfully executed.

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
rows = int(input())
coef = 1

for i in range(1, rows+1):
    for space in range(1, rows-i+1):
        print(" ",end="")
    for j in range(0, i):
        if j==0 or i==0:
            coef = 1
        else:
            coef = coef * (i - j)//j
        print(coef, end = " ")
    print()
```
## Sample Output
<img width="482" height="547" alt="image" src="https://github.com/user-attachments/assets/d548db85-0c0e-41ed-bef6-3cebebe44a59" />

## Result
Thus,the Python program that generates Pascal's Triangle using numbers. The number of rows is accepted from the user is created successfully.

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
num=int(input())
temp = num
count =0
while num>0:
    digit =num%10
    count= count*10+digit
    num//=10
if temp== count:
    print("The given number {} is a Palindrome".format(temp))
else:
    print("The given number {} is not a palindrome".format(temp))

```
## Output
<img width="1070" height="259" alt="image" src="https://github.com/user-attachments/assets/75eda29d-104b-4d01-a48a-87511101e31e" />

## Result
Thus python program to check whether the given number is palindrome or not is executed successfully.
