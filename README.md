num = int(input("Enter a number: "))
if num > 0:
    print("Positive")
elif num < 0:
    print("Negative")
else:
    print("Zero")
2️⃣ Even or Odd
python
num = int(input("Enter a number: "))
if num % 2 == 0:
    print("Even")
else:
    print("Odd")
3️⃣ Voting Eligibility
python
age = int(input("Enter age: "))
if age >= 18:
    print("Eligible to vote")
else:
    print("Not eligible to vote")
4️⃣ Greater of Two Numbers
python
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))
print("Greater number is:", a if a > b else b)
5️⃣ Divisible by 5
python
num = int(input("Enter a number: "))
if num % 5 == 0:
    print("Divisible by 5")
else:
    print("Not divisible by 5")
6️⃣ Multiple of 3
python
num = int(input("Enter a number: "))
if num % 3 == 0:
    print("Multiple of 3")
else:
    print("Not multiple of 3")
7️⃣ Vowel or Consonant
python
ch = input("Enter a character: ").lower()
if ch in "aeiou":
    print("Vowel")
else:
    print("Consonant")
8️⃣ Greater than 100
python
num = int(input("Enter a number: "))
if num > 100:
    print("Greater than 100")
else:
    print("Not greater than 100")
9️⃣ Leap Year
python
year = int(input("Enter a year: "))
if (year % 400 == 0) or (year % 4 == 0 and year % 100 != 0):
    print("Leap year")
else:
    print("Not a leap year")
🔟 Temperature Check
python
temp = float(input("Enter temperature: "))
if temp > 30:
    print("Hot")
else:
    print("Cold")
1️⃣1️⃣ Marks to Grade
python
marks = int(input("Enter marks: "))
if marks >= 90:
    print("Grade A")
elif marks >= 75:
    print("Grade B")
elif marks >= 50:
    print("Grade C")
else:
    print("Fail")
1️⃣2️⃣ Simple Calculator
python
a = float(input("Enter first number: "))
b = float(input("Enter second number: "))
op = input("Enter operator (+, -, *, /): ")

if op == "+":
    print("Result:", a + b)
elif op == "-":
    print("Result:", a - b)
elif op == "*":
    print("Result:", a * b)
elif op == "/":
    print("Result:", a / b if b != 0 else "Error! Division by zero")
else:
    print("Invalid operator")
1️⃣3️⃣ FizzBuzz
python
num = int(input("Enter a number: "))
if num % 3 == 0 and num % 5 == 0:
    print("FizzBuzz")
elif num % 3 == 0:
    print("Fizz")
elif num % 5 == 0:
    print("Buzz")
else:
    print(num)
1️⃣4️⃣ Character Classification
python
ch = input("Enter a character: ")
if ch.isupper():
    print("Uppercase")
elif ch.islower():
    print("Lowercase")
elif ch.isdigit():
    print("Digit")
else:
    print("Special character")
1️⃣5️⃣ Salary Tax
python
salary = int(input("Enter salary: "))
if salary < 250000:
    print("No tax")
elif salary <= 500000:
    print("Tax: 5%")
elif salary <= 1000000:
    print("Tax: 20%")
else:
    print("Tax: 30%")
1️⃣6️⃣ Largest of Three (Nested if)
python
a, b, c = map(int, input("Enter three numbers: ").split())
if a > b:
    if a > c:
        print("Largest:", a)
    else:
        print("Largest:", c)
else:
    if b > c:
        print("Largest:", b)
    else:
        print("Largest:", c)
1️⃣7️⃣ Login System
python
username = input("Enter username: ")
password = input("Enter password: ")

if username == "admin" and password == "12345":
    print("Login successful")
else:
    print("Login failed")
1️⃣8️⃣ Positive → Even/Odd
python
num = int(input("Enter a number: "))
if num > 0:
    if num % 2 == 0:
        print("Positive Even")
    else:
        print("Positive Odd")
else:
    print("Not positive")
1️⃣9️⃣ ATM Withdrawal
python
balance = 10000
withdraw = int(input("Enter withdrawal amount: "))

if withdraw <= balance:
    if withdraw <= 5000:
        balance -= withdraw
        print("Transaction successful. Remaining balance:", balance)
    else:
        print("Withdrawal limit exceeded (max 5000).")
else:
    print("Insufficient balance.")
2️⃣0️⃣ Student Result
python
marks = int(input("Enter marks: "))
if marks >= 35:
    print("Pass")
    if marks >= 75:
        print("Distinction")
    elif marks >= 60:
        print("First Class")
else:
    print("Fail")
2️⃣1️⃣ 3-Digit Number
python
num = int(input("Enter a number: "))
if 100 <= num <= 999:
    print("3-digit number")
else:
    print("Not a 3-digit number")
2️⃣2️⃣ Valid Triangle
python
a, b, c = map(int, input("Enter three angles: ").split())
if a + b + c == 180 and a > 0 and b > 0 and c > 0:
    print("Valid triangle")
else:
    print("Invalid triangle")
2️⃣3️⃣ Second Largest of Three
python
a, b, c = map(int, input("Enter three numbers: ").split())
nums = [a, b, c]
nums.sort()
print("Second largest:", nums[1])
2️⃣4️⃣ Alphabet Check
python
ch = input("Enter a character: ")
if ('a' <= ch <= 'z') or ('A' <= ch <= 'Z'):
    print("Alphabet")
else:
    print("Not an alphabet")
2️⃣5️⃣ Electricity Bill
python
units = int(input("Enter units consumed: "))
bill = 0

if units <= 100:
    bill = 0
elif units <= 200:
    bill = (units - 100) * 5
else:
    bill = (100 * 5) + (units - 200) * 10

print("Electricity Bill:", bill)
2️⃣6️⃣ Movie Ticket Pricing
python
age = int(input("Enter age: "))
if age < 12:
    print("Child Ticket")
elif age > 60:
    print("Senior Ticket")
else:
    print("Adult Ticket")
2️⃣7️⃣ Login with 3 Attempts
python
valid_user = "admin"
valid_pass = "12345"

for attempt in range(3):
    user = input("Enter username: ")
    pwd = input("Enter password: ")
    if user == valid_user and pwd == valid_pass:
        print("Login successful")
        break
    else:
        print("Invalid credentials")
else:
    print("Maximum attempts reached. Access denied.")
2️⃣8️⃣ Palindrome Check
python
num = int(input("Enter a number: "))
if str(num) == str(num)[::-1]:
    print("Palindrome")
else:
    print("Not palindrome")
2️⃣9️⃣ Shopping Discount
python
amount = int(input("Enter shopping amount: "))
if amount >= 5000:
    discount = amount * 0.20
elif amount > 2000:
    discount = amount * 0.10
else:
    discount = 0

print("Discount:", discount)
print("Final amount:", amount - discount)
3️⃣0️⃣ Traffic Signal
python
signal = input("Enter signal color (Red/Yellow/Green): ").lower()
if signal == "red":
    print("Stop")
elif signal == "yellow":
    print("Get Ready")
elif signal == "green":
    print("Go")
else:
    print("Invalid signal")
