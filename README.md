# calculator
def calculator_1(num1, num2):
    command = input("Enter operation: ")
    num1 = int(num1)
    num2 = int(num2)
    match command:
        case "addition":
            print(num1 + num2)
        case "subtraction":
            print(num1 - num2)
        case "division":
            if num2 != 0:
                print(num1 / num2)
            else:
                print("Error: Division by zero!")
        case "multiplication":
            print(num1 * num2)
        case _:
            print("Invalid operation")

num1 = input("Enter the first number: ")
num2 = input("Enter the second number: ")
calculator_1(num1, num2)
