### Week 01: Programming Assignments  

---

### **1. Check if a Number is Even or Odd**  

#### **Task**  
Write a Java program to check if a given integer is even or odd.

#### **Program Code**  
```java
import java.util.Scanner;

public class W01_P1 {
    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        int number = in.nextInt();

        // Check if the number is even or odd
        if (number % 2 == 0) {
            System.out.println("Even");
        } else {
            System.out.println("Odd");
        }
        in.close();
    }
}
```

---

### **2. Calculate the Volume of a Cylinder**  

#### **Task**  
Write a Java program to calculate the volume of a cylinder given its radius and height.  
**Formula:**  
\[
V = \pi \cdot r^2 \cdot h
\]

#### **Program Code**  
```java
import java.util.Scanner;

public class W01_P2 {
    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        double radius = in.nextDouble();
        double height = in.nextDouble();

        // Calculate the volume of the cylinder
        double volume = Math.PI * radius * radius * height;

        System.out.printf("Volume is: %.2f", volume);
        in.close();
    }
}
```

---

### **3. Print Multiplication Table up to 5**  

#### **Task**  
Write a program that takes a number as input and prints its multiplication table up to 5.

#### **Program Code**  
```java
import java.util.Scanner;

public class W01_P3 {
    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        int number = in.nextInt();

        // Print the multiplication table of the number up to 5
        for (int i = 1; i <= 5; i++) {
            System.out.println(number + " x " + i + " = " + (number * i));
        }
        in.close();
    }
}
```

---

### **4. Compute Quotient and Remainder**  

#### **Task**  
Write a program that takes two integers as input and calculates both the quotient and the remainder.

#### **Program Code**  
```java
import java.util.Scanner;

public class W01_P4 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int x = sc.nextInt();
        int y = sc.nextInt();

        // Calculate quotient and remainder
        int quotient = x / y;
        int remainder = x % y;

        System.out.println("The Quotient is = " + quotient);
        System.out.println("The Remainder is = " + remainder);

        sc.close();
    }
}
```

---

### **5. Print a Star Pattern**  

#### **Task**  
Write a program that takes an integer `n` as input and prints the following pattern:  

Example:  
**Input:** `n = 3`  
**Output:**  
```
***
**
*
**
***
```

#### **Program Code**  
```java
import java.util.Scanner;

public class W01_P5 {
    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        int n = in.nextInt();

        // Print the decreasing pattern
        for (int i = n; i > 0; i--) {
            for (int j = 0; j < i; j++) {
                System.out.print("*");
            }
            System.out.println();
        }

        // Print the increasing pattern
        for (int i = 2; i <= n; i++) {
            for (int j = 0; j < i; j++) {
                System.out.print("*");
            }
            System.out.println();
        }

        in.close();
    }
}
```  
