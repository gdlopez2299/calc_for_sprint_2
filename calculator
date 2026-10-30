# By: Gabriel Lopez
# This program is just a basic calculator
# also the old comments sucked so here are some new ones

# this is where the magic happens
def calculate_result(op, num1, num2):
    calculation = 0.0
    # conditionals
    if op == "+":
        calculation = num1 + num2
        print("Operation selected: Addition")
        print("Behind the scenes: {} + {}".format(num1, num2))
    elif op == "-":
        calculation = num1 - num2
        print("Operation selected: Subtraction")
        print("Behind the scenes: {} - {}".format(num1, num2))
    elif op == "*":
        calculation = num1 * num2
        print("Operation selected: Multiplication")
        print("Behind the scenes: {} * {}".format(num1, num2))
    elif op == "/":
        if num2 == 0:
            print("ERROR!!!!!!")
            print("You can't divide anything by zero!")
        else:
            calculation = num1 / num2
            print("Operation selected: Division")
            print("Behind the scenes: {} / {}".format(num1, num2))
    elif op == "//":
        if num2 == 0:
            print("ERROR!!!!!!")
            print("You can't divide anything by zero!")
        else:
            calculation = num1 // num2
            print("Operation selected: Floor division")
            print("Behind the scenes: {} // {}".format(num1, num2))
    elif op == "**":
        calculation = num1 ** num2
        print("Operation selected: Exponent / Power")
        print("Behind the scenes: {} raised to the power of {}".format(num1, num2))
    elif op == "%":
        if num2 == 0:
            print("ERROR!!!")
            print("You can't get any remainders when dividing by 0!")
        else:
            calculation = num1 % num2
            print("Operation selected: Modulo")
            print("Behind the scenes: Remainder of {} divided by {}".format(num1, num2))
    return calculation


# introduction
print("------------------------------------")
print("         GABRIEL'S CALCULATOR       ")
print("------------------------------------")
print("Available operations:")
print("Addittion: + ")
print("Subtraction: - ")
print("Multiplication: * ")
print("Division: / ")
print("Exponent: ** ")
print("Modulo: % ")
print("Floor division: // ")
print("Secret: ???")
print("Type 'quit' to exit.")
print("------------------------------------")
# decided to keep the decorations that I put for extra lines

# just telling the program that yes we want it to run and how many times we have made the function run
calculation_count = 0
running = True

# this ONLY shows if we want the program to keep running
while running:
    # getting whatever operator we will use
    operator = input("Enter operator of your choice (+, -, *, /, **, %, //, ???) or 'quit': ")

    # basically kills the program if we put of these 2 options
    if operator == "quit" or operator == "EXIT":
        running = False
        print("Exiting calculator...")
    else:
        # list of valid operators
        valid_operators = ["+", "-", "*", "/", "//", "**", "%", "???"]

        if operator not in valid_operators:
            print("Error!! You gave the calculator an operator that it does not support!")
            print("You entered: '{}'".format(operator))
            print("Please choose a valid operator symbol!")
        else:
            print("------------------------------------")
            print(" Processing your operator choice...")
            print("------------------------------------")

            # relational operators
            if operator != "???":
                num1 = float(input("Enter your first number: "))
                num2 = float(input("Enter your second number: "))

                if num1 > 1000 or num2 > 1000:
                    print("Note: Working with large numbers.")
                elif not (num1 < 0 and num2 < 0):
                    print("Note: At least one number is non-negative.")

                # function call!!!!
                calculation = calculate_result(operator, num1, num2)
                print("Your result is {}!".format(calculation))

                # shortcut
                calculation_count += 1
            else:
                text = input("Enter text that you want repeated: ")
                repeat_amount = int(input("Enter how many times you want it repeated: "))
                calculation = text * repeat_amount
                print("Operation selected: Secret")
                print("Behind the scenes: {} repeated {} times".format(text, repeat_amount))
                print("Your result is {}!".format(calculation))
                calculation_count += 1

    print("--------------------------------------")

# summary because why not
print("Summary:")
for i in range(1, 2):
    print("You successfully performed {} calculation(s)!!".format(calculation_count))

print(" THANK YOU FOR USING MY CALCULATOR! <3")
