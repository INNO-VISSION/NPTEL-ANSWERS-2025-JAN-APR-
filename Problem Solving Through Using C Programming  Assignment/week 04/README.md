#### Week-04: Program - 01
**Question :**
*Write a C Program to Find the Smallest Number among Three Numbers (integer values) using Nested IF-Else statement.*
##### Source Code:
```
#include <stdio.h>
int main()
{
    int n1, n2, n3; 
    scanf("%d %d %d", &n1, &n2, &n3);
 if (n1 <= n2) {
        if (n1 <= n3) {
            printf("%d is the smallest number.", n1);
        } else {
            printf("%d is the smallest number.", n3);
        }
    } else {
        if (n2 <= n3) {
            printf("%d is the smallest number.", n2);
        } else {
            printf("%d is the smallest number.", n3);
        }
    }

    return 0;
}
```
#### Week-04: Program - 02
**Question :**
*The length of three sides are taken as input. Write a C program to find whether a triangle can be formed or not. If not display “This Triangle is NOT possible.” If the triangle can be formed then check whether the triangle formed is equilateral, isosceles, scalene or a right-angled triangle. (If it is a right-angled triangle then only print Right-angle triangle do not print it as Scalene Triangle)*
##### Source Code:
```
#include<stdio.h>
int main()
{
    int a,b,c; 
    scanf("%d %d %d",&a, &b, &c);
if (a + b > c && a + c > b && b + c > a) {
        if ((a * a + b * b == c * c) || (a * a + c * c == b * b) || (b * b + c * c == a * a)) {
            printf("Right-angle Triangle");
        }
        else if (a == b && b == c) {
            printf("Equilateral Triangle");
        }
        else if (a == b || a == c || b == c) {
            printf("Isosceles Triangle");
        }
        else {
            printf("Scalene Triangle");
        }
    } else {
        printf("Triangle is not possible");
    }
    
    return 0;
}
```
#### Week-04: Program - 03
**Question :**
Write a program to find the factorial of a given number using while loop.

##### Source Code:
```
#include<stdio.h>
void main()
{
    int n;
    long int fact;  
    scanf("%d",&n);
  fact=1;
int i = n;
    while (i > 0) {
        fact *= i;
        i--;
    }
    
    printf("The Factorial of %d is : %ld", n, fact);
}
```
#### Week-04: Program - 04
**Question :**
Write a Program to find the sum of all even numbers from 1 to N where the value of N is taken as input. [For example when N is 10 then the sum is 2+4+6+8+10 = 30]
##### Source Code:
```
#include <stdio.h>  
void main()
{
int N, sum=0; 
scanf("%d", &N);
for (int i = 2; i <= N; i += 2) {
        sum += i;
    }
    
    printf("Sum = %d", sum);
}
```
