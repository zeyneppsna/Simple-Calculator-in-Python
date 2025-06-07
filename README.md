This program takes two numbers and an operator (+, -, *, /) from the user. It performs the chosen arithmetic operation and displays the result. It also handles division by zero and invalid operators.
 ```python
num1 = float(input("Enter first number: "))
op = input("Enter an operator (+, -, *, /): ")
num2 = float(input("Enter second number: "))

if op == '+':
    result = num1 + num2
elif op == '-':
    result = num1 - num2
elif op == '*':
    result = num1 * num2
elif op == '/':
    if num2 != 0:
        result = num1 / num2
    else:
        print("Error: Division by zero!")
        exit()
else:
    print("Invalid operator!")
    exit()

print(f"Result: {result}")
