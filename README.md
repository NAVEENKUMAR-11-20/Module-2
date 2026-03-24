Built-in Functions -Binary Conversion Using Built-in Functions in Python

🎯 Aim

To write a Python program to convert the number 16 into its binary representation using built-in Python functions.

🧠 Algorithm

Assign the value 16 to a variable a.
Use the built-in bin() function to convert the number to binary.
Print the result.

🧾 Program

a = 16
print(bin(a))

Output

<img width="696" height="172" alt="image" src="https://github.com/user-attachments/assets/aae5956b-de1b-4c13-b0c1-8790ebdc9247" />


Result

The program successfully converts the number 16 into its binary representation and prints it.


Functions in Python: Modulo Calculator

🎯 Aim

To write a Python program that defines a function which accepts two values and returns their modulo using the % operator.

🧠 Algorithm

Define a function called result that takes two arguments a and b.
Inside the function, compute the modulo using a % b.
Print the result of the modulo operation.
Get two integer inputs from the user.
Call the result function with the user-provided values.

🧾 Program

def result(a, b):
    return a % b

a = int(input())
b = int(input())
print("The result of the modulo operation is:", result(a, b))

Output

<img width="601" height="194" alt="image" src="https://github.com/user-attachments/assets/e2a6457e-dce5-4c33-a464-0f4ddad0947e" />


Result

The program successfully defines a function that computes the modulo of two numbers and returns the result.



Lambda Function in Python: Addition of Two Numbers

🎯 Aim

To write a Python program that defines a lambda function which takes two arguments a and b, and returns their sum.

🧠 Algorithm

Get two integer inputs from the user.
Use a lambda function to define a function f that returns a + b.
Call the function with the user inputs and print the result.

🧾 Program

i=int(input())
j=int(input())
z=int(input())
f = lambda a, b,c: a+b+c
print(f(i, j,z))


Output

<img width="517" height="402" alt="image" src="https://github.com/user-attachments/assets/486e201e-d78b-43a7-83fd-5b22097b8de4" />

Result

The program successfully defines a lambda function that computes the sum of two numbers and prints the result.



🔺 Looping(Patterns)-Pascal's Triangle Generator in Python

This project demonstrates a simple Python program to generate Pascal’s Triangle, where the number of rows is provided by the user.

🎯 Aim

To write a Python program that generates Pascal's Triangle using numbers. The number of rows is accepted from the user.

🧠 Algorithm

Start the program.
Input the number of rows from the user.
Loop from 0 to the number of rows.
For each row:
Print appropriate spaces to shape the triangle.
Compute values using the formula:
[ C(n, k) = \frac{n!}{k!(n-k)!} ]
Print all rows of Pascal’s Triangle.
End the program.


🧪 Program


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

Output

<img width="637" height="729" alt="image" src="https://github.com/user-attachments/assets/e3825257-6804-4f3a-924d-1b7c6819f160" />



Result

The program successfully generates Pascal's Triangle with the specified number of rows, using the appropriate formula for combination values.



Loops in Python: Palindrome Number Checker

🎯 Aim

To write a Python program that checks whether a given number is a palindrome using loops.


🧠 Algorithm

Get input from the user and assign it to a variable num.
Assign the value of num to a temporary variable temp.
Initialize a variable rev to 0 (used to store the reversed number).
Use a while loop to reverse the digits:
While temp > 0:
rev = (10 * rev) + temp % 10
temp = temp // 10
After the loop, compare rev with num:
If equal, print that the number is a palindrome.
Else, print that it is not a palindrome.


🧾 Program

num = int(input())
temp = num
rev = 0

while temp > 0:
    rev = (10 * rev) + temp % 10
    temp = temp // 10

if rev == num:
    print(f"{num} is a palindrome.")
else:
    print(f"{num} is not a palindrome.")


Output

<img width="1032" height="266" alt="image" src="https://github.com/user-attachments/assets/bb936cb6-645d-4723-90c5-480730379297" />

Result

The program successfully checks if a given number is a palindrome by reversing its digits and comparing it to the original number.
