Basic Python Scripts

---

### 1. **Hello, World!**
A classic first program that prints "Hello, World!" to the console.

```python
print("Hello, World!")
```

**Explanation**:  
- The `print()` function displays the specified message or output to the screen.

---

### 2. **Basic Calculator**
A script that adds two numbers entered by the user.

```python
# Taking input from the user
num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number: "))

# Adding the numbers
sum = num1 + num2

# Displaying the result
print("The sum is:", sum)
```

**Explanation**:  
- `input()` is used to take input from the user.
- `float()` converts the input into a floating-point number to handle decimals.
- The sum is calculated and printed.

---

### 3. **Check if a Number is Even or Odd**
A script that determines if a number is even or odd.

```python
# Taking input from the user
num = int(input("Enter a number: "))

# Checking if the number is even or odd
if num % 2 == 0:
    print("The number is even.")
else:
    print("The number is odd.")
```

**Explanation**:  
- `%` (modulus operator) checks the remainder.
- If the remainder is zero when dividing by 2, the number is even; otherwise, it's odd.

---

### 4. **Simple Interest Calculator**
Calculates simple interest given the principal, rate, and time.

```python
# Taking input from the user
principal = float(input("Enter principal amount: "))
rate = float(input("Enter interest rate: "))
time = float(input("Enter time in years: "))

# Calculating simple interest
interest = (principal * rate * time) / 100

# Displaying the result
print("The simple interest is:", interest)
```

**Explanation**:  
- Simple interest formula: \[ \text{Interest} = \frac{\text{Principal} \times \text{Rate} \times \text{Time}}{100} \]
- We calculate interest and display it.

---

### 5. **Find the Largest of Three Numbers**
Finds the largest among three numbers entered by the user.

```python
# Taking input from the user
num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number: "))
num3 = float(input("Enter third number: "))

# Finding the largest number
if num1 >= num2 and num1 >= num3:
    largest = num1
elif num2 >= num1 and num2 >= num3:
    largest = num2
else:
    largest = num3

# Displaying the result
print("The largest number is:", largest)
```

**Explanation**:  
- We use `if-elif-else` statements to check each condition and find the largest number.

---

### 6. **Factorial of a Number**
Calculates the factorial of a number using a loop.

```python
# Taking input from the user
num = int(input("Enter a number: "))
factorial = 1

# Calculating factorial
for i in range(1, num + 1):
    factorial *= i

# Displaying the result
print("The factorial of", num, "is:", factorial)
```

**Explanation**:  
- The `for` loop multiplies each number up to `num` to calculate the factorial.

---

### 7. **Fibonacci Series up to n Terms**
Generates the Fibonacci sequence up to `n` terms.

```python
# Taking input from the user
n = int(input("Enter number of terms: "))

# First two terms
a, b = 0, 1
count = 0

# Generating Fibonacci sequence
while count < n:
    print(a, end=" ")
    a, b = b, a + b
    count += 1
```

**Explanation**:  
- `a` and `b` represent the first two terms of the Fibonacci series.
- Each iteration calculates the next term and prints it.

---

### 8. **Check if a String is a Palindrome**
Checks if a string reads the same forward and backward.

```python
# Taking input from the user
string = input("Enter a string: ")

# Checking if the string is a palindrome
if string == string[::-1]:
    print("The string is a palindrome.")
else:
    print("The string is not a palindrome.")
```

**Explanation**:  
- `string[::-1]` reverses the string.
- If the original string is equal to the reversed string, it’s a palindrome.

---

### 9. **Prime Number Checker**
Checks if a number is prime or not.

```python
# Taking input from the user
num = int(input("Enter a number: "))

# Checking if the number is prime
if num > 1:
    for i in range(2, int(num**0.5) + 1):
        if num % i == 0:
            print("The number is not prime.")
            break
    else:
        print("The number is prime.")
else:
    print("The number is not prime.")
```

**Explanation**:  
- A prime number has only two divisors: 1 and itself.
- We check divisibility up to the square root of the number to optimize performance.

---

### 10. **Counting Vowels in a String**
Counts the number of vowels in a given string.

```python
# Taking input from the user
string = input("Enter a string: ")

# Defining vowels
vowels = "aeiouAEIOU"
count = 0

# Counting vowels
for char in string:
    if char in vowels:
        count += 1

# Displaying the result
print("The number of vowels in the string is:", count)
```

**Explanation**:  
- We loop through each character in the string, checking if it's a vowel.
- If so, we increment the `count` and display it at the end.

