### Week 2: Programming Assignment 1

#### 1. Create a Python program that calculates the sum of the squares of the first n natural numbers. The program should prompt the user to input a number n, then compute and print the sum of squares from 1 to n.
**Program Code :**

n = int(input())


sum_of_squares = sum(i ** 2 for i in range(1, n + 1))


print(sum_of_squares)
---
### Week 2: Programming Assignment 2

#### 2. Write a Python program to calculate the arithmetic mean of n numbers, rounding the result to the nearest integer. The program should first take a single line of input containing n space-separated integer numbers, and then output the rounded mean of these numbers.
**Program Code :**

numbers = list(map(int,input().split()))

if len(numbers)<1:

  Print("No Number is Provided")
  
else:

  mean=round(sum(numbers)/len(numbers))
print(mean)
  
---
### Week 2: Programming Assignment 3

#### 3. Develop a Python program that determines the mode of a list of n numbers, assume only one mode exists in the provided test cases. The program should ask for a single line of input containing n, then n space-separated numbers, and output the mode.

**Program Code :**

from collections import Counter

input_data = input().split()

n = int(input_data[0])
numbers = list(map(int, input_data[1:]))

if len(numbers) != n:
    print("Error: The number of values does not match the count specified.")
else:
    frequency = Counter(numbers)
    mode = max(frequency, key=frequency.get)
    print(mode)
