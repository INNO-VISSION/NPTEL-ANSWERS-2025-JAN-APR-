### Week 6: Programming Assignment 1
**Question**
*The Treasure Hunt*

You are part of an elite team of treasure hunters, and your latest mission is to find the hidden treasure in a mysterious ancient temple. Inside the temple, you discover a series of enchanted scrolls containing arrays of magical numbers. The numbers are encrypted in different arrays, and each scroll has a clue indicating which element in the array holds the key to the treasure.

You are given one of these arrays, and the clue on the scroll tells you that the treasure is hidden inside the kth smallest number in that array. Your task is to figure out the kth smallest number from the array, where k is smaller than the size of the array, and return it as your answer.

The treasure huntes in your team trust you with this task, and the sooner you find the key, the sooner they can open the vault. So, be efficient and find the answer quickly!
**Source Code*
```
def find_kth_smallest(arr, k):
    n = len(arr)
    if k > n:
        return 'The clue k should be smaller than or equal to the list size'
    
    arr.sort()
    return arr[k-1]

# Dynamic Input
arr = list(map(int, input("").split()))
k = int(input(""))

# Output the result
print(find_kth_smallest(arr, k))
```
#### Programming Assignment 2
**Question**
*The Binary Quest*

Alex, a young programmer, discovered a challenge: Convert a decimal number to binary using recursion! The rules were simple—no loops, no built-in functions —only the magic of recursion.

 Steps to convert a decimal number to binary:

·       Divide the number by 2.

·       Store the remainder (0 or 1).

·       Repeat with the quotient until it becomes 0.

·       Read the remainders in reverse order to get the binary number.
**Source Code*
```
def decimal_to_binary(n):
    if n == 0:
        return '0'
    if n == 1:
        return '1'
    return decimal_to_binary(n // 2) + str(n % 2)

n = int(input())
print(decimal_to_binary(n))
```
#### Programming Assignment 3
**Question**
Removing an element Recursively:

Write a recursive function delete_elements in Python that removes all occurrences of a specified item from a list, creating and returning a new list without modifying the input list.
**Source Code*
```
def delete_elements(lst, item):
    if not lst:
        return []
    if lst[0] == item:
        return delete_elements(lst[1:], item)
    else:
        return [lst[0]] + delete_elements(lst[1:], item)
      
lst = list(map(int,input().split(' ')))
item = int(input())
new_lst=delete_elements(lst,item)
print(*new_lst, end='')
````
