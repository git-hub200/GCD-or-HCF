# GCD-or-HCF
#For 2 input numbers
"""n1=int(input("Enter number1: "))
n2=int(input("Enter number2: "))
fact=1
for i in range(1,min(n1,n2)+1):
    if n1%i==0 and n2%i==0:
        fact=i
print(f"GCD of {n1}, {n2} is {fact}")"""


#For n no.of input numbers
number=list(map(int,input("Enter numbers to find GCD: ").split(",")))
fact=1
for i in range(1,min(number)+1):
    if all(num%i ==0 for num in number):
        fact=i
num_str=",".join(map(str,number))
print(f"GCD of {num_str} is {fact}")
