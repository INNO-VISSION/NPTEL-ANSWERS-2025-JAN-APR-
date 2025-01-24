### Week 2: Assignment - Programming in Java  

### Questions and Answers  

1. **Consider the following object declaration statement: Scanner in = new Scanner(System.in); What does System.in stand for in the above declaration?**  
   Options:  
   a. Any file storing data  
   b. Refers to the standard input stream, which is typically the keyboard by default.  
   c. Reference to Scanner as an input device  
   d. It is a mouse as an input device  
   *Answer*: b. Refers to the standard input stream, which is typically the keyboard by default.  
---
2. *What will be the output of the following Java program?*
   
   public class VarPrint {
   
       int x = 30;
       static int y = 20;
       public static void main(String[] args) {
           VarPrint t1 = new VarPrint();
           t1.x = 88;
           t1.y = 99;
           int z1 = t1.x + t1.y;
           VarPrint t2 = new VarPrint();
           System.out.println(t2.x + " " + t2.y + " " + z1);
   
       }
   
   }
     
   Options:  
   a. 30 99 178  
   b. 30 88 129  
   c. 30 99 187  
   d. 88 99 178  
   *Answer*: c. 30 99 187    
---
3. *What will be the output of the following Java program?*
   
   public class ArgsOverTest {
   
       public static void main(String[] args) {
           Test t = new Test();
           t.start();
   
       }
       static class Test {
           void start() {
               int a = 4;
               int b = 5;
               System.out.print("" + 8 + 3 + "");
               System.out.print(a + b);
               System.out.print(" " + a + b + "");
               System.out.print(foo() + a + b + " ");
               System.out.println(a + b + foo());
           }
           String foo() {
               return "foo";
           }
       }
   
   }
     
   Options:  
   a. 9 7 7 foo34 34foo  
   b. 839 45foo45 9foo  
   c. 72 34 34 foo34 34foo  
   d. 9 7 7 foo 7 7foo  
   *Answer*: b. 839 45foo45 9foo   
---
4. *What is encapsulation in object-oriented programming?*  
   Options:  
   a. Hiding implementation details and exposing only functionality  
   b. The process of creating multiple objects in a program  
   c. Writing multiple methods in a single class  
   d. Using the this keyword to reference an object  
   *Answer*: a. Hiding implementation details and exposing only functionality  
---
5. *Which of the following is true about constructors in a class?*  
   Options:  
   a. Constructors must have a return type.  
   b. Constructors are used to initialize objects.  
   c. A class can have only one constructor.  
   d. Constructors cannot be overloaded.  
   *Answer*: b. Constructors are used to initialize objects.  
---
6. **What does the this keyword in Java help to achieve?**  
   Options:  
   a. Avoiding namespace collision between instance variables and method parameters  
   b. Overloading methods in a class  
   c. Accessing private methods in another class  
   d. Creating multiple objects in a program  
   *Answer*: a. Avoiding namespace collision between instance variables and method parameters  
---
7. **What is the correct signature of the main method in Java?**  
   Options:  
   a. public void main(String arg[])  
   b. public static void main(String arg[])  
   c. void main(String[] arg)  
   d. public static void main(String[] args)  
   *Answer*: d. public static void main(String[] args)  
---
8. *Which of the following is used to take input from Java?*  
   Options:  
   a. BufferedReader  
   b. Scanner  
   c. DataInputStream  
   d. All of the above  
   *Answer*: d. All of the above  
---
9. *Which method is used to format output in Java?*  
   Options:  
   a. print()  
   b. println()  
   c. printf()  
   d. format()  
   *Answer*: c. printf()  
---
10. *Which Java class is primarily used to read input from the console?*  
    Options:  
    a. Scanner  
    b. BufferedReader  
    c. Console  
    d. DataInputStream  
    *Answer*: a. Scanner
