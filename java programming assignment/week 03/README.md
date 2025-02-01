### Week 03: Programming Assignment 1 - Programming in java

Write a program to print the factorial of a number by defining a *static recursive method* named Factorial.

The factorial of a number n is represented by n! and is equal to 1 * 2 * 3 * ... * (n-1) * n. For example:
- 4! = 1 * 2 * 3 * 4 = 24
- 3! = 3 * 2 * 1 = 6
- 2! = 2 * 1 = 2
Also,
- 1! = 1
- 0! = 1

---

#### Solution Code

import java.util.Scanner;

class W03_P1 {
    
    public static int factorial(int n) {
        
        if (n == 0 || n == 1) {
            return 1;
        }
        
        return n * factorial(n - 1);
    }

    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        int x;
        x = in.nextInt(); 
        System.out.print(factorial(x)); 
    }
}

# Week 03: Programming Assignment 2

There are two class cls1 and cls2 which is subclass of cls1.  cls1 having a method "add" which add two numbers. Create two method inside cls2 which will take 2 parameters as input i.e. a and b and print the sum , multiplication and sum of their squares i.e (a^2) + (b^2) (name the function task())

---

## Solution Code

import java.util.Scanner;

class W03_P1 {
    
    public static int factorial(int n) {
        
        if (n == 0 || n == 1) {
            return 1;
        }
        
        return n * factorial(n - 1);
    }

    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        int x;
        x = in.nextInt(); 
        System.out.print(factorial(x)); 
    }
}

# Week 03: Programming Assignment 3

Complete the code segment to count number of digits in an integer using while loop.

(Remember to match the output given exactly, including the spaces and new lines)

---

## Solution Code

import java.util.Scanner;

public class W03_P3 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int num = sc.nextInt();
        
        
        int count = 0;
        
        
        if (num == 0) {
            count = 1;
        } else {
            
            while (num != 0) {
                num /= 10;
                count++;
            }
        }
        
        System.out.println(count);
        
        sc.close();
    }
}



