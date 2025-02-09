#### Week 04:  Programming In Java

##### 1. Which access modifier allows a method to be accessible within the same package but not from outside the package?  
   - A. default  
   - B. private  
   - C. public  
   - D. protected  
   *Answer:* A. default  
   *Explanation:* The default access modifier allows methods to be accessed only within the same package.

##### 2. What will happen if you attempt to access a private method from another class in Java?  
   - A. The method will be accessible.  
   - B. The method will throw an exception.  
   - C. The method will be inaccessible.  
   - D. The method will be converted to protected.  
   *Answer:* C. The method will be inaccessible.  
   Explanation: Private methods can only be accessed within the class where they are defined.

##### 3. What will be the output of the following code?  
```
class Person {
    int a = 1;
    int b = 0;
    public Person() {
        System.out.println(a + b + " Java ");
    }
}
class Employee extends Person {
    int a = 0;
    int b = 1;
    public Employee() {
        System.out.println(a * b + " Java ");
    }
}
public class Question {
    public static void main(String args[]) {
        Person p = new Employee();
    }
}
```
   - A. Java 10

        0 Java  

   - B. 1 Java
   
         0 Java  

   - C. 10 Java 
        
        0 Java  
   - D. 1 Java 1 
        
        0 Java  

   *Answer:* B. 1 Java
                0 Java

##### 4. Which of the following is a built-in Java package?  
   - A. java.util  
   - B. my.package.util  
   - C. default.package  
   - D. system.java  
   *Answer:* A. java.util  
   *Explanation:* java.util is a standard built-in package in Java.

##### 5. What keyword is used to define a package in Java?  
   - A. define  
   - B. package  
   - C. import  
   - D. namespace  
   *Answer:* B. package  
   *Explanation:* The package keyword is used to declare a package in Java.

##### 6. How do you import a specific class from a package in Java?  
   - A. import package.*;  
   - B. import package.ClassName;  
   - C. include package.ClassName;  
   - D. use package.ClassName;  
   *Answer:* B. import package.ClassName;  
   *Explanation:* This syntax imports a specific class from a package.

##### 7. Consider the following program: How many errors does this program contain?  
```
class Base {
    public void print() {
        System.out.println("Base class...");
    }
}

class Derived extends Base {
    public void print() {
        System.out.println("Derived class...");
    }
}

public class Main {
    private static void main(String[] args) {
        Base b = new Base();
        b.print();
        Derived d = new Derived();
        d.print();
    }
}

```
   - A. None  
   - B. 1  
   - C. 2  
   - D. 3  
   *Answer:* A. None  
   *Explanation:* The program is error-free as per the syntax and logic.

##### 8. Which of the following is true about Java interfaces?  
   - A. They cannot contain method implementations.  
   - B. An interface can extend multiple classes.  
   - C. An interface can only contain abstract methods.  
   - D. They allow a class to achieve multiple inheritance.  
   *Answer:* D. They allow a class to achieve multiple inheritance.  
   *Explanation:* Java interfaces enable multiple inheritance, as a class can implement multiple interfaces.

##### 9. What will happen if you do not specify an access modifier for a class in a package?  
   - A. The class will be 'private' by default.  
   - B. The class will be 'protected' by default.  
   - C. The class will be accessible only within the same package.  
   - D. The class will be 'public' by default.  
  *Answer:*C. The class will be accessible only within the same package.  
  *Explanation:* The default access level allows accessibility only within the same package.

##### 10. Which access modifier provides the most restrictive access in Java?  
`
    - A. default  
    - B. protected  
    - C. private  
    - D. public  
    *Answer:* C. private  
    *Explanation:* The private modifier restricts access to within the same class only.
