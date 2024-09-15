number_list=[]
name=input("enter your name:")
print()
for i in range(1,4):
num=int(input(f"Enter your {i} favorite number: "))
number_list.append(num)

print(f"\nHello, {name}! let's explore your favorite number:")
for num in number_list:
if num % 2 == 0:
print (f"The number {num} is even.")
else:
print (f"The number {num} is odd.")
print()
for num in number_list:
print(f"The number (num) and its square: ((num), {num \*\*2})")
sum_numbers= sum(number_list)
print(f"\n Here is the sum of your favorite numbers: {sum_numbers}")
if sum_numbers==0 or sum_numbers==1:
print(num, "is not a prime number")
elif sum_numbers > 1:
for i in range(2, sum_numbers):
if (num % i) == 0:
prime = True

if prime:
print(f"Alas! {sum_numbers}, is not a prime number")
else:
print(f"Wow! {sum_numbers}, is a prime number")
