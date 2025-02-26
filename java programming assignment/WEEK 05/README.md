### **Week 05: Programming Assignment 1 - Programming in java** 
An interface Number is defined in the following program.

You have to declare a class A, which will implement the interface Number
```
import java.util.Scanner;

interface Number {
    int findSqr(int i);  
}

class A implements Number {
    
    public int findSqr(int i) {
        return i * i;  square
    }
}

public class W05_P1 { 
    public static void main(String[] args) { 
        A a = new A();   
        Scanner sc = new Scanner(System.in);
        
        int i = sc.nextInt();
        
        System.out.print(a.findSqr(i));
    } 
}

```
---
### **Week 05: Programming Assignment 2 - Programming in java** 
This program is to find the GCD (greatest common divisor) of two integers writing a recursive function findGCD(n1,n2).


Your function should return -1, if the argument(s) is(are) negative (zero is allowed).
```
import java.util.Scanner;

interface GCD {
    public int findGCD(int n1, int n2);
}

// Create a class B, which implements the interface GCD
class B implements GCD {
    public int findGCD(int n1, int n2) {
        if (n1 < 0 || n2 < 0) {
            return -1;
        }
        if (n2 == 0) {
            return n1;
        }
        return findGCD(n2, n1 % n2);
    }
}

public class W05_P2 {
    public static void main(String[] args) {
        B a = new B(); // Create an object of class B
        Scanner sc = new Scanner(System.in);

        int p1 = sc.nextInt();
        int p2 = sc.nextInt();

        System.out.print(a.findGCD(p1, p2));
    }
}

```
---

### **Week 05: Programming Assignment 3 - Programming in java**  

Complete the code segment to catch the ArithmeticException in the following, if any.

On the occurrence of such an exception, your program should print “Exception caught: Division by zero.”


If there is no such exception, it will print the result of division operation on two integer values. 
```
import java.util.Scanner;

public class W05_P3 {
    public static void main(String[] args) { 
        int a, b;
        Scanner input = new Scanner(System.in);
        
        int result;

        a = input.nextInt();
        b = input.nextInt();
        
        try {
            
            result = a / b;
            System.out.print(result);
        } catch (ArithmeticException e) {
            
            System.out.print("Exception caught: Division by zero.");
        }
    }
}

```

---

### **Week 05: Programming Assignment 4 - Programming in java**  

In the following program, an array of integer data to be initialized.

During the initialization, if a user enters a value other than integer value, then it will throw InputMismatchException exception.

On the occurrence of such an exception, your program should print “You entered bad data.”


If there is no such exception it will print the total sum of the array..
```
import java.util.Scanner;
import java.util.InputMismatchException;

public class W05_P4 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int length = sc.nextInt(); 
        
        int[] name = new int[length];
        int sum = 0;

        try {
            // Loop to read array elements
            for (int i = 0; i < length; i++) {
                name[i] = sc.nextInt();
                sum += name[i]; 
            }
            System.out.print(sum); 
        } catch (InputMismatchException e) {
            System.out.print("You entered bad data."); 
        }
    }
}

```
---

### **Week 05: Programming Assignment 5 - Programming in java**  

 In the following program, there may be multiple exceptions.

```
import java.util.Scanner;

public class W05_P5 {
    public static void main(String args[]) {
        Scanner scan = new Scanner(System.in);
        int i = scan.nextInt();
        int j;

        try {
            switch (i) {
                case 0:
                    int zero = 0;
                    j = 92 / zero;  
                    break;
                case 1:
                    int b[] = null;
                    j = b[0];      
                    break;
                default:
                    System.out.print("No exception");
            }
        } catch (Exception e) {
            System.out.print(e);  
        }
    }
}

```
---
