## **Week 5: Programming In Java**  

##### **1. Which of the following statement(s) is/are true about `finally` in Java?**

I. The `finally` block is executed regardless of whether an exception is thrown or not.  
II. A `finally` block can exist without a `catch` block.  
III. The `finally` block will not execute if `System.exit()` is called in the `try` block.  
IV. A `finally` block can have a `return` statement, but it is not recommended to use.

a. I and II  
b. II and III  
c. I, II and III  
d. I, II, III and IV  

**Answer: d. I, II, III and IV**  

---

##### **2. **What will be the output of the following Java program?**

```java
interface A {
    int x = 10;
    void display();
}

class B implements A {
    public void display() {
        System.out.println("Value of x: " + x);
    }
}

public class Main {
    public static void main(String[] args) {
        B obj = new B();
        obj.display();
    }
}
```
a. Value of x: 10  

b. Value of x: 0

c. Compilation Error  

d. Runtime Error

**Answer:** a. Value of x: 10

---

##### **3. What will be the output of the following program?**

```java
class NPTEL {
    public static void main(String[] args) {
        try {
            int a = 5;
            int b = 0;
            System.out.println(a / b);
        } catch (ArithmeticException e) {
            System.out.print("Error ");
        } finally {
            System.out.print("Complete");
        }
    }
}
```

---

a. 5 Complete  
b. Error Complete  
c. Runtime Error  
d. Compilation Error

**Answer:** b. Error Complete  

---

##### **4. Which of the following is TRUE regarding abstract class and an interface in Java?**  

I. Abstract classes can contain constructors, but interfaces cannot.  
II. Interfaces support multiple inheritance, but abstract classes do not.  
III. Abstract classes can have both abstract and concrete methods, whereas interfaces only had abstract methods before Java 8.  

A. I, II and III  
B. II only  
C. I and II only  
D. II and III only  

**Answer:** A. I, II and III  

---

##### **5. Which of the following is a _checked exception_ in Java?**  

a. NullPointerException  
b. ArrayIndexOutOfBoundsException  
c. IOException  
d. ArithmeticException  

**Answer:** c. IOException 

---

##### **6. Which keyword is NOT used by Java during exception handling?**  

a. try  
b. catch  
c. final  
d. finally  

**Answer:** c. final  

---

##### **7. What is the purpose of the `throws` keyword in Java?**  

a. To declare exceptions that a method can throw  
b. To throw an exception immediately  
c. To catch an exception  
d. It is not a keyword in Java  

**Answer:** a. To declare exceptions that a method can throw  

---

##### **8. Which of the following is TRUE about interfaces in Java?**  

a. Interfaces should always be defined as final  
b. Interfaces can be instantiated directly  
c. Interfaces can extend multiple interfaces  
d. Interfaces cannot have any method signatures  

**Correct Answer:** c. Interfaces can extend multiple interfaces   

---

##### **9. What will be the output of the following code?**  

```java
interface Demo {  
    void display();  
}  

class Test implements Demo {  
    public void display() {  
        System.out.println("Hello, NPTEL!");  
    }  
}  

public class Main {  
    public static void main(String[] args) {  
        Test obj = new Test();  
        obj.display();  
    }  
}
```

a. Hello, NPTEL!  
b. Compilation Error  
c. Runtime Error  
d. No Output  

**Answer:** a. Hello, NPTEL!  

---

##### **10. What will be the output of the following Java program?**  

```java
interface Calculator {  
    void calculate(int value);  
}  

class Square implements Calculator {  
    int result;  
    public void calculate(int value) {  
        result = value * value;  
        System.out.print("Square: " + result + " ");  
    }  
}  

class Cube extends Square {  
    public void calculate(int value) {  
        result = value * value * value;  
        super.calculate(value);  
        System.out.print("Cube: " + result + " ");  
    }  
}  

public class Main {  
    public static void main(String[] args) {  
        Calculator obj = new Cube();  
        obj.calculate(3);  
    }  
}
```

a. Square: 9 Cube: 9  
b. Cube: 27 Square: 9  
c. Square: 9 Square: 27 Cube: 27  
d. Square: 9 Cube: 27   

**Answer:** d. Square: 9 Cube: 27  

---
