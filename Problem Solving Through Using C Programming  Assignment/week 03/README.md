### Week-03: Program-01

#### Write a C Program to calculates the area (floating point number with two decimal places) of a Circle given it’s radius (integer value). The value of Pi is 3.14.
##### Source Code :

#include <stdio.h>

#define PI 3.14

void main()

{

    int radius;
    float area;
    /* Enter the radius of a circle */
    scanf("%d", &radius);
    area = PI * radius * radius;
    printf("Area of a circle = %5.2f\n", area);
}

#### Week-03: Program-02

#### Write a C program to check if a given Number is zero or Positive or Negative Using if...else statement
##### Source Code :

#include <stdio.h>

int main()

{

    double number;
    scanf("%lf", &number); 
      if (number > 0)
    {
        printf("Positive number.");
    }
    else if (number < 0)
    {
        printf("Negative number.");
    }
    else
    {
        printf("The number is 0.");
    }

    return 0;
}

#### Week-03: Program-03

Write a C program to check whether a given number (integer) is Even or Odd.
##### Source Code :

#include <stdio.h>

int main()

{
    int number;
    scanf("%d", &number);
    if (number%2 == 0)
    {
  printf("%d is even.",number);
  
}
else 
{
  printf("%d is odd.",number);
}
}

### Week-03 Program-04

#### Write a C Program to find the Largest Number (integer) among Three Numbers (integers) using IF and Logical && operator.
##### Source Code :

#include <stdio.h>

int main()
{
    int n1, n2, n3;

    scanf("%d %d %d", &n1, &n2, &n3); 

    if (n1 >= n2 && n1 >= n3)
    {
        printf("%d is the largest number.", n1);
    }
    else if (n2 >= n1 && n2 >= n3)
    {
        printf("%d is the largest number.", n2);
    }
    else
    {
        printf("%d is the largest number.", n3);
    }

    return 0;
}
