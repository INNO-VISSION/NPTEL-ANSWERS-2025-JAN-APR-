### Week 3: Programming Assignment 1
#### 1. Create a Python program that finds the second smallest number in a list of positive integers (including zero). The program should prompt the user to input a list of numbers, then compute and print the second smallest number in that list.

**Program Code :**
```

def find_second_smallest(numbers):

    unique_numbers = sorted(set(numbers))
    
    if len(unique_numbers) > 1:
        return unique_numbers[1]
    else:
        return "No second smallest number"
input_numbers = input()

number_list = list(map(int, input_numbers.split()))

second_smallest = find_second_smallest(number_list)

print(second_smallest)
```

### Week 3: Programming Assignment 2
#### 2. Create a Python program that removes even duplicate positive integer numbers(includes zero) from a list and prints the unique numbers in the order they first appeared.
The program should prompt the user to input a list of numbers, then process the list to remove duplicates and print the resulting list of unique numbers.

**Program Code :**
```
def remove_even_duplicates(numbers):
    seen = set()
    result = []
    
    for num in numbers:
        if num % 2 == 0 and num not in seen:
            seen.add(num)
            result.append(num)
        elif num % 2 != 0:
            result.append(num)
    
    return result

input_numbers = input()

number_list = list(map(int, input_numbers.split()))

unique_numbers = remove_even_duplicates(number_list)

print(" ".join(map(str, unique_numbers)))
```
### Week 3: Programming Assignment 3
#### 3. Create a Python program that takes a list of integers, reverses the list, adds the values at even indices from both the original and reversed lists, and creates a new list with the result. The new list should be printed in the end.

**Program Code:**
```
def process_list(nums):
    
    reversed_nums = nums[::-1]
    
    
    result = [nums[i] + reversed_nums[i] if i % 2 == 0 else nums[i] for i in range(len(nums))]
    
    return result

input_list = list(map(int, input().split()))

output = process_list(input_list)

print(*output)
```

