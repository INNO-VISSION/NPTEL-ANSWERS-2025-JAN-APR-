## **Week 7:  Java Programming Assignment**


1. **Implement a Simple Calculator**
A Calculator class is provided. Your task is to implement the following:

A parameterized constructor to initialize two numbers.

Methods for addition, subtraction, multiplication, and division.

The division method should handle division by zero and print "Cannot divide by zero!" if attempted.

Follow the naming conventions in the given template code.

```
import java.util.Scanner;

class W07_1 {
    private int num1;
    private int num2;

    // Constructor to initialize num1 and num2
    public W07_1(int num1, int num2) {
        this.num1 = num1;
        this.num2 = num2;
    }

    // Method for addition
    public int add() {
        return num1 + num2;
    }

    // Method for subtraction
    public int subtract() {
        return num1 - num2;
    }

    // Method for multiplication
    public int multiply() {
        return num1 * num2;
    }

    // Method for division with zero handling
    public int divide() {
        if (num2 == 0) {
            System.out.println("Cannot divide by zero!");
            return 0; // Default return value to prevent crash
        }
        return num1 / num2;
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int a = scanner.nextInt();
        int b = scanner.nextInt();

        W07_1 calc = new W07_1(a, b);
        System.out.println("Sum: " + calc.add());
        System.out.println("Difference: " + calc.subtract());
        System.out.println("Product: " + calc.multiply());
        System.out.println("Quotient: " + calc.divide());

        scanner.close();
    }
}

```

---

2. **Implement a Simple Calculator**
A Calculator class is provided. Your task is to implement the following:

A parameterized constructor to initialize two numbers.

Methods for addition, subtraction, multiplication, and division.

The division method should handle division by zero and print "Cannot divide by zero!" if attempted.

Follow the naming conventions in the given template code.

```
import java.util.Scanner;

class Counter {
    private int count;

    // Constructor to initialize count to zero
    public Counter() {
        this.count = 0;
    }

    // Method to increment count by 1
    public void increment() {
        count++;
    }

    // Method to decrement count by 1 but ensure it does not go below zero
    public void decrement() {
        if (count > 0) {
            count--;
        }
    }

    // Method to get the current value of count
    public int getValue() {
        return count;
    }
}

public class W07_2 {
    public static void main(String[] args) {
        Counter counter = new Counter();

        counter.increment();
        counter.increment();
        counter.decrement();

        System.out.println(counter.getValue()); // Output: 1
    }
}
```
---

3. **Implement a Basic Employee Class**
An Employee class is provided. Implement:

A constructor to initialize name and salary.

A method getDetails() to return "Employee: Name, Salary: X" format.

Example Input:
Alice 50000
Example Output:

```
import java.util.Scanner;

class Employee {
    private String name;
    private double salary;

    // Constructor to initialize name and salary
    public Employee(String name, double salary) {
        this.name = name;
        this.salary = salary;
    }

    // Method to return employee details in the required format
    public String getDetails() {
        return "Employee: " + name + ", Salary: " + salary;
    }
}

public class W07_3 {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        String empName = scanner.next();
        double empSalary = scanner.nextDouble();

        Employee emp = new Employee(empName, empSalary);
        System.out.print(emp.getDetails());

        scanner.close();
    }
}
```

---

4. **mplement a Simple Array Processor**
You need to complete the implementation of the getMax() method inside the NumberArray class. This method should return the largest number from the array.

Tasks:
Complete the getMax() method in the template section.
The method should iterate through the array and find the largest value.
**Example Input:**
3 8 1 5 7
**Example Output:**
Max: 8, Min: 1

```
import java.util.Scanner;

// Class to store and process an array of numbers
class NumberArray {
    private int[] numbers; // This array will store the numbers given by the user

    // Constructor to initialize the array
    public NumberArray(int[] numbers) {
        this.numbers = numbers;
    }

    // Method to find the maximum value in the array
    public int getMax() {
        int max = numbers[0]; // Assume first element is the max
        for (int num : numbers) {
            if (num > max) {
                max = num;
            }
        }
        return max;
    }

    // Method to find the minimum value in the array
    public int getMin() {
        int min = numbers[0]; // Assume first element is the min
        for (int num : numbers) {
            if (num < min) {
                min = num;
            }
        }
        return min;
    }
}

// Main class to test the NumberArray class
public class W07_4 {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Read 5 integers from the user and store them in an array
        int[] arr = new int[5]; // Create an array of size 5
        for (int i = 0; i < arr.length; i++) {
            arr[i] = scanner.nextInt(); // Read numbers from user
        }

        // Create an instance of NumberArray and print max & min values
        NumberArray numArray = new NumberArray(arr);
        System.out.println("Max: " + numArray.getMax() + ", Min: " + numArray.getMin());

        scanner.close(); // Close scanner to free resources
    }
}
```
---
5. **Implement a Simple Password Validator**
In this task, you need to implement a password validation system using Java. The goal is to check if a given password meets the following conditions:

Minimum Length Requirement: The password must be at least 8 characters long.
Uppercase Letter Requirement: The password must contain at least one uppercase letter (A-Z).
Number Requirement: The password must contain at least one numeric digit (0-9).
If the password meets all three conditions, print "Valid Password". Otherwise, print "Invalid Password".


**Input Format:**
A single string representing the password (can contain alphabets, numbers, and special characters).
Output Format:
Print "Valid Password" if the password satisfies all the conditions.
Otherwise, print "Invalid Password".

**Example Input:**
Password123


**Example Output:**
Valid Password

```
import java.util.Scanner;

public class W07_5 {
    private String password;

    // Constructor to initialize the password variable
    public W07_5(String password) {
        this.password = password;
    }

    // Method to check if the password is valid
    public boolean isValidPassword() {
        if (password.length() < 8) {
            return false;
        }

        boolean hasUpperCase = false;
        boolean hasDigit = false;

        for (char ch : password.toCharArray()) {
            if (Character.isUpperCase(ch)) {
                hasUpperCase = true;
            }
            if (Character.isDigit(ch)) {
                hasDigit = true;
            }
        }

        return hasUpperCase && hasDigit;
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        // Read password input from user
        String inputPassword = scanner.nextLine();

        W07_5 validator = new W07_5(inputPassword);

        // Check password validity and print result
        if (validator.isValidPassword()) { // Removed the incorrect argument
            System.out.print("Valid Password");
        } else {
            System.out.print("Invalid Password");
        }

        scanner.close();
    }
}
```

---
