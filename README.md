print("===== MATHEMATICAL CALCULATOR =====")

while True:
    print("\nChoose an operation")
    print("+  Addition")
    print("-  Subtraction")
    print("*  Multiplication")
    print("/  Division")
    print("// Floor Division")
    print("%  Modulus")
    print("^  Power")
    print("C  Clear")
    print("OFF Exit")

    choice = input("Enter your choice: ")

    if choice == "OFF":
        print("Calculator Closed.")
        break

    elif choice == "C":
        print("\nScreen Cleared")
        continue

    elif choice in ["+", "-", "*", "/", "//", "%", "^"]:
        num1 = float(input("Enter first number: "))
        num2 = float(input("Enter second number: "))

        if choice == "+":
            print("Answer =", num1 + num2)

        elif choice == "-":
            print("Answer =", num1 - num2)

        elif choice == "*":
            print("Answer =", num1 * num2)

        elif choice == "/":
            if num2 == 0:
                print("Division by zero is not allowed.")
            else:
                print("Answer =", num1 / num2)

        elif choice == "//":
            if num2 == 0:
                print("Division by zero is not allowed.")
            else:
                print("Answer =", num1 // num2)

        elif choice == "%":
            if num2 == 0:
                print("Division by zero is not allowed.")
            else:
                print("Answer =", num1 % num2)

        elif choice == "^":
            print("Answer =", num1 ** num2)

    else:
        print("Invalid Choice")
