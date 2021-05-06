# python-projects - Brand name Generator!

# a = input("a:")
# b = input("b:")

# c = a
# a = b
# b = c


# print("a = " + a)
# print("b = " + b)


print("Hello Everyone Welcome to Brand Name Generator!")
city = input("Which city you grew up in\n")
petName = input("What is your pet name\n")
print ("Your brand name could be "+ city +" "+ petName)


# Calculator code

#Addition
def add(n1,n2):
  return n1 + n2

# Substract
def subtract(n1,n2):
  return n1 - n2  

# Multiply
def multiply(n1,n2):
  return n1 * n2

# Divide
def divide(n1,n2):
  return n1 / n2

operations = {
  "+": add,
  "-": subtract,
  "*": multiply,
  "/":divide
}  

num1 = int(input("Enter the first number: "))


for symbol in operations:
  print(symbol)
operation_symbol = input("Pick and operation symbol: ") 
num2 = int(input("Enter the second number: ")) 
  
calculation_function = operations[operation_symbol]
answer = calculation_function(num1,num2)


print(f"{num1} {operation_symbol} {num2} = {answer}")


# Calculator code with while loop.

#Addition
def add(n1,n2):
  return n1 + n2

# Substract
def subtract(n1,n2):
  return n1 - n2  

# Multiply
def multiply(n1,n2):
  return n1 * n2

# Divide
def divide(n1,n2):
  return n1 / n2

operations = {
  "+": add,
  "-": subtract,
  "*": multiply,
  "/":divide
}  

num1 = int(input("Enter the first number: "))


for symbol in operations:
  print(symbol)
should_continue = True  

while should_continue:
  operation_symbol = input("Pick and operation symbol: ") 
  num2 = int(input("Enter the next number: ")) 
  
  calculation_function = operations[operation_symbol]
  answer = calculation_function(num1,num2)

  print(f"{num1} {operation_symbol} {num2} = {answer}")

  if input(f"Enter 'y' to continue with {answer}. Enter 'n' to exit: ") == "y":
    num1 = answer
  else:
    should_continue = False
    
    
 #Completed Calculator Code.
 
 from replit import clear
from art import logo

def add(n1, n2):
  return n1 + n2

def subtract(n1, n2):
  return n1 - n2

def multiply(n1, n2):
  return n1 * n2

def divide(n1, n2):
  return n1 / n2

operations = {
  "+": add,
  "-": subtract,
  "*": multiply,
  "/": divide
}

def calculator():
  print(logo)

  num1 = float(input("What's the first number?: "))
  for symbol in operations:
    print(symbol)
  should_continue = True
 
  while should_continue:
    operation_symbol = input("Pick an operation: ")
    num2 = float(input("What's the next number?: "))
    calculation_function = operations[operation_symbol]
    answer = calculation_function(num1, num2)
    print(f"{num1} {operation_symbol} {num2} = {answer}")

    if input(f"Type 'y' to continue calculating with {answer}, or type 'n' to start a new calculation: ") == 'y':
      num1 = answer
    else:
      should_continue = False
      clear()
      calculator()



    

