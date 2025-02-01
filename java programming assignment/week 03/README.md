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
# Week 03: Programming Assignment 4

A Student class with private fields (name, age) is provided,

Your task is to make the following: 

- a parameterized constructor to initialize the private fields

- the getter/setter methods for each field

Follow the naming convention as given in the main method of the suffix code.

---

## Solution Code

import java.util.Scanner;

class Student {
    
    private String name;
    private int age;

    
    public Student(String name, int age) {
        this.name = name;
        this.age = age;
    }

    
    public String getName() {
        return name;
    }

    
    public void setName(String name) {
        this.name = name;
    }

    
    public int getAge() {
        return age;
    }

   
    public void setAge(int age) {
        this.age = age;
    }

    
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        
        String name = scanner.next();
        int age = scanner.nextInt();

        
        Student student = new Student(name, age);

        
        System.out.print("Name: " + student.getName() + ", Age: " + student.getAge());

        scanner.close();
    }
}
# Week 03: Programming Assignment 5

This program is an exercise to call static and non-static methods.

A partial code is given defining two methods, namely sum( ) and multiply ( ).

You have to call these methods to find the sum and product of two numbers.

Complete the code segment as instructed.  

---

## Solution Code


import java.util.Scanner;

class QuestionScope {

    int sum(int a, int b) { 
        return a + b;
    }

    static int multiply(int a, int b) { 
        return a * b;
    }
}

public class W03_P5 {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n1 = sc.nextInt();
        int n2 = sc.nextInt();

        QuestionScope st = new QuestionScope();
        int result1 = st.sum(n1, n2); 
        int result2 = QuestionScope.multiply(n1, n2); 
        
        System.out.println(result1);
        System.out.print(result2);
    }
}





