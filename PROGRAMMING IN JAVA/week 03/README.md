# Week 3 Assignment 3 - Programming in Java

## Questions and Answers

### 1. Which of the following is true about the super keyword in Java? 
  a. super can be used to call a parent class constructor.  
  b. super is used to access private variables of the parent class.  
  c. super is used to call a static method in the parent class.  
  d. super can only be used inside a static method.  
*Answer:* a. super can be used to call a parent class constructor.

### 2. What is the output of the following Java program?

class StaticScopeDemo {
    static int x = 5;

    public static void main(String[] args) {
        int x = 10;
        {
            int x = 15; 
            System.out.println(x); 
        }
        
    }
}

 
  a. 15  
  b. Compilation Error  
  c. 5  
  d. 10  
*Answer:* a. 15

### 3. What will be the output of the following program?

class Parent {
    void display() {
        System.out.println("Parent display");
    }
}

class Child extends Parent {
    void display() {
        System.out.println("Child display");
    }
}

public class Main {
    public static void main(String[] args) {
        Parent obj = new Child();
        obj.display();
    }
}


  a. Parent display  
  b. Child display  
  c. Compilation Error  
  d. Runtime Error  
*Answer:* b. Child display

### 4. Which of the following statements about abstract classes in Java is correct?
  
  a. Abstract classes can be instantiated directly.  
  b. An abstract class must contain at least one abstract method.  
  c. A class inheriting from an abstract class must implement all its abstract methods unless it is itself abstract.  
  d. Abstract classes can be marked as final.  
*Answer:* c. A class inheriting from an abstract class must implement all its abstract methods unless it is itself abstract.

### 5. What will be the output of the following Java program?

public class NptelExample {
    public static int fun(int n) {
        if (n == 0) {
            return 1;
        }
        return n * fun(n - 1);
    }
    public static void main(String[] args) {
        System.out.println(fun(5));
    }
}


  a. 5  
  b. 24  
  c. 120  
  d. Runtime Error  
*Answer:* c. 120

### 6. Which of the following is NOT true regarding the final keyword in Java?

  a. A final method cannot be overridden in a subclass.  
  b. A final variable can only be assigned once.  
  c. A final class can have subclasses.  
  d. A final variable can be assigned during declaration or in the constructor.  
*Answer:* c. A final class can have subclasses.

### 7. What is the output of the following Java program?

class Test {
    static int count = 0;
    public Test() {
        count++;
    }
    public static void main(String[] args) {
        Test obj1 = new Test();
        Test obj2 = new Test();
        Test obj3 = new Test();
        System.out.println("Count: " + Test.count);
    }
}

 
  a. Count: 0  
  b. Compilation Error  
  c. Runtime Error  
  d. Count: 3  
*Answer:* d. Count: 3

### 8. Which of these is NOT an example of method overriding in Java?

  a. A subclass defining a method with the same name but different parameters than a superclass method.  
  b. A subclass providing a new implementation for a method in the superclass.  
  c. A subclass defining a method with the same name and parameters as a superclass method.  
  d. Using the super keyword to call the superclass version of an overridden method.  
*Answer:* a. A subclass defining a method with the same name but different parameters than a superclass method.

### 9. What is the output of the following Java program?

class Parent {
    String message() {
        return "Parent";
    }
}
class Child extends Parent {
    String message() {
        return "Child";
    }
}
public class Main {
    public static void main(String[] args) {
        Child p = new Parent();
        System.out.println(p.message());
    }
}

 
  a. Parent  
  b. Child  
  c. Compilation Error  
  d. No error and nothing is printed  
*Answer:* c. Compilation Error

### 10. What is the output of the following program?

public class Nptel {
    public static int fun(int n) {
        if (n == 0) {
            return 0;
        }
        return n + fun(n - 1);
    }
    public static void main(String[] args) {
        System.out.println(fun(5));
    }
}

 
  a. 5  
  b. 10  
  c. 15  
  d. Runtime Error  
*Answer:* c. 15

