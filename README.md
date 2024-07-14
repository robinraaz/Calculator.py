# Calculator.py
def calculator():
    # Take input from the user
    num1 = float(input("Enter the 1st number: "))
    num2 = float(input("Enter the 2nd number: "))
    op = input("Enter an operation (+, -, *, /): ")
    # Define a function to perform the calculation based on the operator
    def calculate(num1, num2, op):
        if op == '+':
            return num1 + num2
        elif op == '-':
            return num1 - num2
        elif op == '*':
            return num1 * num2
        elif op == '/':
            if num2 != 0:
                return num1 / num2
            else:
                return "Error: Division by zero is not allowed."
        else:
            return "Invalid operation"
    
    # Perform the calculation and print the result
    result = calculate(num1, num2, op)
    print(f"The result of {num1} {op} {num2} is: {result}")

# Run the calculator
calculator()
