# pythonpart2
#updating calculator functions
import re
def add(numbers)
    ans=numbers[0]+numbers[1]
    return ans

def subtract(numbers)
    ans=numbers[0]-numbers[1]
    return ans

def multiply(numbers)
    ans=numbers[0]*numbers[1]
    return ans

def divide(numbers)
    ans=numbers[0]/numbers[1]
    return ans

calculation = input("Type your calculation")

numbers = []
numbers = re.findall(r'\d+', calculation)
print(numbers)

for x in calculation:
    if x == "+":
        ans = add(numbers)
    elif x == "-":
        subtract(numbers)
    elif x == "*":
        multiply(numbers)
    elif x == "/":
        divide(numbers)
    else:
        print("error")

