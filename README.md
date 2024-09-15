# Python Programming Assignment #
# Number Exploration Tool #
## Instructions ##
### Step 1: Initialize Variables ###
We will initialize an empty list to store the user's favorite numbers and prompt for their name:

number_list = []
name = input("Enter your name: ")

### Step 2: Loop for Number Input ###
We will use a for loop to ask the user for three numbers and add them to the number_list.
 for i in range(1, 4):
 
    num = int(input(f"Enter your favorite number {i}: "))
    number_list.append(num)
    
### Step 3: Print Greeting ###
We will greet the user by printing their name.

for num in number_list:

    if num % 2 == 0:
        print(f"The number {num} is even.")
    else:
        print(f"The number {num} is odd.")
        
### Step 5: Print Even/Odd ###
We will print the result of the even/odd check directly as part of the loop from step 4.
### Step 6: Print Number and Square ###
We will print each number and its square using another loop.

print()

for num in number_list:

    print(f"The number {num} and its square: ({num}, {num ** 2})")
    
### Step 7: Calculate Sum of Numbers ###
We will calculate the sum of all the numbers in number_list:

sum_numbers = sum(number_list)

### Step 8: Print Sum ###
We will print the sum of the favorite numbers:

print(f"\nHere is the sum of your favorite numbers: {sum_numbers}")

### Step 9: Prime Check for Edge Cases ###
We will check if the sum is 0 or 1 and print that it is not a prime number.

if sum_numbers == 0 or sum_numbers == 1:

    print(f"{sum_numbers} is not a prime number.")

    
### Step 10: Prime Check Logic ###
We will check whether the sum is divisible by any number from 2 to sum_numbers-1. If it is, then the sum is not prime.

elif sum_numbers > 1:

    prime = True
    for i in range(2, sum_numbers):
    
        if sum_numbers % i == 0:
        
            prime = False
            break
            
### Step 11: Print Prime or Not Prime ###
We will print whether the sum is a prime number based on the prime check from step 10.

if prime:

    print(f"Wow! {sum_numbers} is a prime number.")
    
else:

    print(f"Alas! {sum_numbers} is not a prime number.")
    
### Step 12: End Program ###
The program ends after printing the prime check result. There's no additional code needed for this step

