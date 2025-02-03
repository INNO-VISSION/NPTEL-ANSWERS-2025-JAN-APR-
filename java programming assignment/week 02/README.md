### Week 02 : Programming Assignment 1

Write a Java program to create a class Student with the following attributes: name, age, and grade. Create a constructor to initialize these attributes. Display the student’s information using a method displayInfo().

---
##### Solution Code


import java.util.*;

class Student {

    String name;
    int age;
    String grade;

    public Student(String name, int age, String grade) {
        this.name = name;
        this.age = age;
        this.grade = grade;
    }

    public void displayInfo() {
        System.out.println("Student Name: " + name);
        System.out.println("Age: " + age);
        System.out.print("Grade: " + grade);
    }
}

public class W02_P1 {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String name = sc.nextLine();
        int age = sc.nextInt();
        String grade = sc.next();

        Student student = new Student(name, age, grade);
        student.displayInfo();

        sc.close();
    }
}

### Week 02 : Programming Assignment 2

Write a program that demonstrates constructor overloading. Create a class Student with two constructors:

1. A constructor that accepts name and age 
2. A constructor that accepts all three attributes: name, age, and grade.
Print the student's information using a method displayInfo().

---
#### Solution Code

import java.util.*;

class Student {

    String name;
    int age;
    String grade;

    public Student(String name, int age, String grade) {
        this.name = name;
        this.age = age;
        this.grade = grade;
    }

    public void displayInfo() {
        System.out.println("Student Name: " + name);
        System.out.println("Age: " + age);
        System.out.print("Grade: " + grade);
    }
}

public class W02_P1 {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String name = sc.nextLine();
        int age = sc.nextInt();
        String grade = sc.next();

        Student student = new Student(name, age, grade);
        student.displayInfo();

        sc.close();
    }
}

### Week 02 : Programming Assignment 3

Write a program to demonstrate the use of this keyword. Create a class Rectangle with attributes length and breadth. Write a constructor to initialize these values. Also, define a method area() to return the area of the rectangle.

---
#### Solution Code

import java.util.*;

public class W02_P3 {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int length = sc.nextInt();
        int breadth = sc.nextInt();

        // Define the class Rectangle here
        class Rectangle {
            int length, breadth;

            // Constructor
            Rectangle(int length, int breadth) {
                this.length = length;
                this.breadth = breadth;
            }

            // Method to calculate area
            int area() {
                return length * breadth; // Correct formula
            }
        }


### Week 02 : Programming Assignment 4

Create a class Car with attributes brand and price. Add a method display() to show the car details. Write a program to create two objects of this class and display their details.

---
#### Solution Code

import java.util.*;

public class W02_P4 {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String brand1 = sc.next();
        int price1 = sc.nextInt();
        String brand2 = sc.next();
        int price2 = sc.nextInt();

        // Define the class Car here
        class Car {
            // Variables
            String brand;
            int price;

            // Constructor
            Car(String brand, int price) {
                this.brand = brand;
                this.price = price;
            }

            // Display method
            void display(int num) {
                System.out.println("Car " + num + ": " + brand + ", Price: " + price);
            }
        }

        // Create two objects of Car and display their details
        Car car1 = new Car(brand1, price1);
        Car car2 = new Car(brand2, price2);

        car1.display(1);
        car2.display(2);

        sc.close();
    }
}

        // Create an object of Rectangle and call the area method
        Rectangle r = new Rectangle(length, breadth);
        System.out.print(r.area());

        sc.close();
    }
}

### Week 02 : Programming Assignment 5

Write a Java program to demonstrate the concept of encapsulation by modeling a Book object. The program should include methods for setting and getting the title and author of the book, and a method to display the details of the book.

*Task:*

1. Create a class Book with the following private attributes:

- title (String)
- author (String)
2. Include the following methods in the Book class:

- setTitle(String title) to set the title of the book.
- setAuthor(String author) to set the author of the book.
- getTitle() to return the title of the book.
- getAuthor() to return the author of the book.
- displayDetails() to print the details of the book in the format

Title: <title>  
Author: <author>  

3. In the main() method, create an object of the Book class, set the title and author, and then call the displayDetails() method to print the book details.
---
#### Solution Code
```
import java.util.Scanner;

public class W02_P5 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        String title = sc.next();
        String author = sc.next();
        
        // Create a Book object
        Book book = new Book();
        
        // Set title and author
        book.setTitle(title);
        book.setAuthor(author);
        
        // Display book details
        book.displayDetails();
        
        sc.close();
    }
}

// Define the Book class with private attributes for title and author
class Book {
    // Private attributes
    private String title;
    private String author;
    
    // Setter for title
    public void setTitle(String title) {
        this.title = title;
    }
    
    // Setter for author
    public void setAuthor(String author) {
        this.author = author;
    }
    
    // Getter for title
    public String getTitle() {
        return this.title;
    }
    
    // Getter for author
    public String getAuthor() {
        return this.author;
    }

    // Method to display details
    public void displayDetails() {
        System.out.println("Title: " + this.title);
        System.out.println("Author: " + this.author);
    }
}
