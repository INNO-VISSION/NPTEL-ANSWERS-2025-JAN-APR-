## **Week 8:  Java Programming Assignment**

1.  **Write a Java program that reads a positive integer from the user and computes the sum of its digits.**
 
**Expected Input/Output:**

 Input: 123

 Output: 6
 ```
 import java.util.Scanner;

public class W08_P1 {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter a positive integer: ");
        int number = scanner.nextInt(); 
        int sum = 0;
        while (number > 0) {
            int digit = number % 10;  
            sum += digit;             
            number /= 10;             
        }
        System.out.println(sum);
        scanner.close();
    }
}
```
---

2. **Write a Java program that reads an integer from the user and computes its factorial.**
Factorial of a number n is calculated as: n! = n * (n-1) * (n-2) * ... * 1, 
 Assume the input is a non-negative integer.
 ```
 import java.util.Scanner;

public class W08_P2 {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter a non-negative integer: ");
        int n = scanner.nextInt();

        long factorial = 1;

        if (n == 0) {
            factorial = 1;
        } else {
            
            for (int i = 1; i <= n; i++) {
                factorial *= i;
            }
        }

        System.out.println(factorial);

        scanner.close();
    }
}

```

3. **Write a Java program that reads a positive integer from the user and prints its reverse.**

Expected Input/Output:

 Input: 1234

 Output: 4321

```
import java.util.Scanner;

public class W08_P3 {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        
        System.out.print("Enter a positive integer: ");
        int number = scanner.nextInt();
        int reversedNumber = 0;
        while (number != 0) {
            int digit = number % 10;  
            reversedNumber = reversedNumber * 10 + digit;  
            number = number / 10;  
        }
        System.out.println(reversedNumber);
        scanner.close();
    }
}

```
---

4. **Write a Java program that reads an integer and determines if it is a prime number.**
 A prime number is only divisible by 1 and itself.

Expected Input/Output:

Input: 7

Output: Prime 

```
import java.util.Scanner;

public class W08_P4 {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter an integer: ");
        int number = scanner.nextInt();
        boolean isPrime = true;
        if (number <= 1) {
            isPrime = false;
        } else {
            for (int i = 2; i <= Math.sqrt(number); i++) {
                if (number % i == 0) {
                    isPrime = false;
                    break; 
                }
            }
        }

        if (isPrime) {
            System.out.println("Prime");
        } else {
            System.out.println("Not Prime");
        }
        scanner.close();
    }
}

```

5. **Write a Java program to perform matrix multiplication.**
The program should:
 - Read two matrices from user input.
 - Validate that matrix multiplication is possible (columns of first == rows of second).
 - Compute the product of the matrices.
 - Display the resulting matrix.
 
  Expected Input/Output:

  Input:
  2 3  \ (Rows and Columns of first matrix)
  1 2 3
  4 5 6
  3 2  \ (Rows and Columns of second matrix)
  7 8
  9 10
  11 12

  Output:
  58 64
  139 154
 ----------------------
 Input:
 2 2
 1 2
  3 4
  2 2
  2 0
  1 3

  Output:
  4 6

  10 12

```
import java.util.Scanner;

public class W08_P5 {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int rows1 = scanner.nextInt();
        int cols1 = scanner.nextInt();
        int[][] matrix1 = new int[rows1][cols1];

        for (int i = 0; i < rows1; i++) {
            for (int j = 0; j < cols1; j++) {
                matrix1[i][j] = scanner.nextInt();
            }
        }

        int rows2 = scanner.nextInt();
        int cols2 = scanner.nextInt();
        int[][] matrix2 = new int[rows2][cols2];
        for (int i = 0; i < rows2; i++) {
            for (int j = 0; j < cols2; j++) {
                matrix2[i][j] = scanner.nextInt();
            }
        }
        if (cols1 != rows2) {
            System.out.println("Multiplication Not Possible");
            return;
        }
        int[][] result = new int[rows1][cols2];
        for (int i = 0; i < rows1; i++) {
            for (int j = 0; j < cols2; j++) {
                for (int k = 0; k < cols1; k++) {
                    result[i][j] += matrix1[i][k] * matrix2[k][j];
                }
            }
        }
        for (int i = 0; i < rows1; i++) {
            for (int j = 0; j < cols2; j++) {
                System.out.print(result[i][j]);
                if (j < cols2 - 1) {
                    System.out.print(" ");
                }
            }
            System.out.println(); 
        }

        scanner.close();
    }
}
```


