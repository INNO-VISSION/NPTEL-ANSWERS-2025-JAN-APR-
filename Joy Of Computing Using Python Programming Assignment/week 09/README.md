### Week 9: Programming Assignment 1

### Question:
We represent scores of batsmen across a sequence of matches in a two-level dictionary as follows:

{'match1’: {'player1':57, 'player2':38}, 'match2’: {'player3':9, 'player1':42}, 'match3’: {'player2':41, 'player4':63, 'player3':91}

 **Source Code : **
 
```
def orangecap(d):
    scores = {}
    
    for match in d.values():
        for player, score in match.items():
            scores[player] = scores.get(player, 0) + score
    
    top_player = max(scores, key=scores.get)
    return (top_player, scores[top_player])
```
### Week 9: Programming Assignment 2
### Question:
A positive integer m can be expressed as the sum of three squares if it is of the form p + q + r where p, q, r ≥ 0, and p, q, r are all perfect squares. For instance,
2 can be written as 0+1+1 but 7 cannot be expressed as the sum of three squares. The first numbers that cannot be expressed as the sum of three squares are 7, 15, 23, 28, 31, 39, 47, 55, 60, 63, 71, …(see Legendre's three-square theorem).

 **Source Code : **
 ```

def threesquares(m):
    if m <= 0:
        return False
    
    while m % 4 == 0:
        m //= 4
    
    if m % 8 == 7:
        return False

    for i in range(int(m**0.5) + 1):
        for j in range(int((m - i*i)**0.5) + 1):
            k = (m - i*i - j*j)
            if k >= 0 and (k**0.5).is_integer():
                return True

    return False
```
### Week 9: Programming Assignment 3
### Question:
A list of numbers is said to be a hill if it consists of an ascending sequence followed by a descending sequence, where each of the sequences is of length at least two. Similarly, a list of numbers is said to be a valley if it consists of an descending sequence followed by an ascending sequence. You can assume that consecutive numbers in the input sequence are always different from each other.


Write a Python function hillvalley(l) that takes a list l of integers and returns True if it is a hill or a valley, and False otherwise.

 **Source Code : **
 ```
def hillvalley(l):
    if len(l) < 4:
        return False

    i = 1

    # Check for increasing sequence (Hill) or decreasing sequence (Valley)
    while i < len(l) and l[i] > l[i - 1]:
        i += 1

    if i == 1 or i == len(l):  
        return False  

    peak_or_trough = i  

    # Check for decreasing sequence (Hill) or increasing sequence (Valley)
    while i < len(l) and l[i] < l[i - 1]:
        i += 1

    return i == len(l)  
  ```
