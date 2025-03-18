### Week 8: Programming Assignment 1
**Question**
##### Remove Strings from a List of Tuples

You are given a list of tuples, where each tuple contains a mix of integers and strings. Your task is to remove all string elements from each tuple while keeping the original structure of the list.

·       If a tuple becomes empty after removing strings, it should be represented as an empty tuple ().

·       The number of tuples in the output list must be the same as in the input list.

Input Format:

A list of tuples

Output Format:

A list of tuples with all string elements removed.
**Source Code**
```
import ast

input_data = ast.literal_eval(input())  
output_data = list(tuple(item for item in tup if not isinstance(item, str)) for tup in input_data)

print(output_data)
```
### Week 8: Programming Assignment 2
**Question**
##### Remove Anagram Duplicates and Sort

You are given a sequence of words. Two words are anagrams if they contain the same letters in a different order. Your task is to remove any word that is an anagram of an earlier word while keeping the first occurrence. Finally, print the remaining words in sorted order.

Input Format:

A single line containing space-separated words, where each word consists of lowercase letters only.

Output Format:

A single line containing the remaining words in sorted order, space-separated.

Example:

Input:

code doce ecod framer frame

Output:

code frame framer
**Source Code**
```
words = input().split()
seen = set()
unique_words = []

for word in words:
    sorted_word = ''.join(sorted(word))
    if sorted_word not in seen:
        seen.add(sorted_word)
        unique_words.append(word)

print(" ".join(sorted(unique_words)))
```
### Week 8: Programming Assignment 3
**Question**
##### Multiply Adjacent Elements in a Tuple

In many data processing tasks, cumulative operations like summation or multiplication of adjacent elements are required. This problem focuses on adjacent element multiplication, where each pair of consecutive elements in a given tuple is multiplied to generate a new tuple. The input tuple can contain both positive and negative integers, and the goal is to compute a resultant tuple where each element is the product of two adjacent elements in the original tuple.

 

Input Format:

A tuple of integers T with n elements (n ≥ 2)

Output Format:

A new tuple R of size (n - 1) where each element R[i] is the product of T[i] and T[i+1].
**Source Code**
```
T = tuple(map(int, input().strip("()").split(",")))
R = tuple(T[i] * T[i + 1] for i in range(len(T) - 1))
print(R)
```

