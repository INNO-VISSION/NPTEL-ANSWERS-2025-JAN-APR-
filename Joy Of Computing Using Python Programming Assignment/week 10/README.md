### Week 10: Programming Assignment 1
### Question:
Emma is a budding software developer working on a signal detection system. One day, her mentor gives her a special list called nums. This list only contains two types of signals:

1 represents a strong signal.
0 represents a weak signal.

 **Source Code :**
 
 ```
def findMaxConsecutiveOnes(nums):
    max_count = 0  # To store the maximum streak of 1s
    current_count = 0  # To count the current streak of 1s
    
    for num in nums:
        if num == 1:
            current_count += 1  # Increment count if 1 is found
            max_count = max(max_count, current_count)  # Update max streak
        else:
            current_count = 0  # Reset count when a 0 is found
    
    return max_count
```
### Week 10: Programming Assignment 2
### Question:
In the ancient land of Lexiconia, hidden messages are locked behind a common magical prefix. Only those who can decipher the longest common prefix will unveil the wisdom of the lost texts.

Your task is to create a function that accepts a list of words, finds the longest common prefix, and prints the result.

 **Source Code :**
 
 ```
def longestCommonPrefix(st):
    if not st:
        return "\"\""
    
    # Sort the list to bring similar prefixes together
    st.sort()
    
    # Compare the first and last word (which will have the least in common)
    first, last = st[0], st[-1]
    prefix = ""
    
    for i in range(min(len(first), len(last))):
        if first[i] == last[i]:
            prefix += first[i]
        else:
            break
    
    return f'"{prefix}"'
```
### Week 10: Programming Assignment 3
### Question:
Once upon a time in the land of Isomorphia, there were two ancient scrolls written in different languages. The wise king of Isomorphia wanted to know if these scrolls conveyed the same message or if they were completely different. He summoned his greatest coder, who had the magical power of Isomorphic Translation.

 **Source Code :**
 
 ```
def isIsomorphic(s, t):
    if len(s) != len(t):
        return False
    
    s_to_t = {}
    t_to_s = {}
    
    for char_s, char_t in zip(s, t):
        if char_s in s_to_t:
            if s_to_t[char_s] != char_t:
                return False
        else:
            s_to_t[char_s] = char_t
        
        if char_t in t_to_s:
            if t_to_s[char_t] != char_s:
                return False
        else:
            t_to_s[char_t] = char_s
    
    return True
```



