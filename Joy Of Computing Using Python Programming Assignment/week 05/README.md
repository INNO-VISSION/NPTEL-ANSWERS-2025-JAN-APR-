### Week 4: Programming Assignment 1
**Question :**
You are tasked with analyzing a mysterious message that was intercepted. The message seems to contain a series of repeated words, and the challenge is to count how many times each word appears. To solve this, you must write a Python program that takes a string of text and counts the frequency of each word.

Make sure your program is case-insensitive, as the secret message is a mix of upper and lower case letters.

After counting the occurrences of each word, display the results.


Input Format:  A line of text

Output format: For all the unique words in the sentence, word: followed by frequency.

#### Source Code:
```
import string
from collections import OrderedDict

def count_word_frequency(text):
    # Remove punctuation and convert to lowercase
    text = text.translate(str.maketrans("", "", string.punctuation)).lower()
    words = text.split()
    
    # Use OrderedDict to preserve order
    word_counts = OrderedDict()
    for word in words:
        word_counts[word] = word_counts.get(word, 0) + 1

    return word_counts

# Taking input
input_text = input()

# Counting word frequency
frequency = count_word_frequency(input_text)

# Printing the results
for word, count in frequency.items():
    print(f"{word}: {count}")
```
### Programming Assignment 2
**Question :**

Merging Dictionaries

You are required to write a Python function merge_dicts that takes two dictionaries as input and returns a new dictionary containing all the entries from both input dictionaries. The function should not modify the input dictionaries.

The dictionaries will have strings as keys and numbers as values. In the case where the same key appears in both dictionaries, the corresponding value in the output dictionary should be the sum of the values from both dictionaries.


You need to ensure the following:

If a key exists in only one of the dictionaries, its value should remain the same in the result.

If a key exists in both dictionaries, sum the values associated with that key.

The output dictionary should include all the keys from both input dictionaries, with updated values as described above.
**Input Format:**
Two dictionaries containing string keys and numerical values in two separate lines.
**Output Format:**
A new dictionary containing all the entries from both the dictionaries, with values summed for common keys

#### Sources Code:

def merge_dicts(d1, d2):
```
   #your code goes here
    merged = dict1.copy()
    for key, value in dict2.items():
        merged[key] = merged.get(key, 0) + value
    return merged
```
def parse_input(input_string):
    input_string = input_string.strip('{}').strip()
    parsed_dict = {}
    if input_string:
        items = input_string.split(',')
        for item in items:
            key, value = item.split(':')
            key = key.strip().strip("'").strip('"') 
            value = int(value.strip())  
            parsed_dict[key] = value    
    return parsed_dict

if __name__ == "__main__":
    dict1_input = input()
    dict2_input = input()
    dict1 = parse_input(dict1_input)
    dict2 = parse_input(dict2_input)
    merged_dict = merge_dicts(dict1, dict2)
    print("Merged Dictionary:", merged_dict)
    
### Programming Assignment 3

**Question :**
Sorting the Royal Manuscripts

You are an apprentice in the Royal Library of the Vijayanagara Empire, home to centuries-old ancient manuscripts filled with knowledge on astronomy, Ayurveda, and warfare. However, a strong monsoon wind has scattered the manuscripts in random order!

The Rajguru (Royal Scholar) assigns you a crucial task: sort the manuscripts using the ancient "Bubble Sort" technique. But there’s a rule—you must record the order of manuscripts after every pass, as the Rajguru wishes to witness the sorting magic unfold gradually.

Your sorting spell, called "Grantha Sudharaka" (Sacred Manuscript Arranger), can swap two manuscripts at a time, ensuring the heaviest ones settle at the bottom after each pass. Your goal is to restore order to the library as quickly as possible. If there are no swaps, you can stop the process of arranging.

Can you help bring back order to the Royal Library of Vijayanagara?

Input Format :

List of integers separated by spaces.

Output Format :

Every pass output in a single line.
#### Source Code:
```
def grantha_sudharaka(manuscripts):
    n = len(manuscripts)

    for i in range(n - 1):  # Loop for each pass
        swapped = False

        for j in range(n - 1 - i):  # Compare adjacent elements
            if manuscripts[j] > manuscripts[j + 1]:
                manuscripts[j], manuscripts[j + 1] = manuscripts[j + 1], manuscripts[j]  # Swap
                swapped = True
        
        print(" ".join(map(str, manuscripts)))  # Print current state after each pass

        if not swapped:  # If no swaps were made, list is sorted
            break

# Taking input
manuscripts = list(map(int, input().split()))

# Calling the function
grantha_sudharaka(manuscripts)
```
    

