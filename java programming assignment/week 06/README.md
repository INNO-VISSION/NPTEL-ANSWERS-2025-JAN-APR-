## **Week 6:  Programming Assignment**


1. **Complete the code segment to print the following using the concept of extending the Thread class in Java:**

-----------------OUTPUT-------------------

Thread is Running.

-------------------------------------------------
```
.
public class W06_P1 extends Thread {   
    public void run() {               
        System.out.print("Thread is Running."); 
    }

    public static void main(String args[]) {
        
        W06_P1 thread = new W06_P1();
        
        thread.start();
    }
}
```
---

2. **In the following program, a thread class ThreadRun is created using the Runnable interface which prints "Thread using Runnable interface". Complete the main class to create a thread object of the class ThreadRun and run the thread**

```
class ThreadRun implements Runnable {
    public void run() { 
        System.out.print("Thread using Runnable interface."); 
    } 
}

public class W06_P2 {
    public static void main(String[] args) {
      
        ThreadRun runnable = new ThreadRun();
        
     
        Thread thread = new Thread(runnable);
        
        thread.start();
    }
}

```
---

3. **A part of the Java program is given, which can be completed in many ways, for example using the concept of thread, etc.  Follow the given code and complete the program so that your program prints the message "NPTEL Java". Your program should utilize the given interface/ class.**
```
// Interface A is defined with an abstract method run()
interface A {
    public abstract void run();
}

// Class B is defined which implements A and an empty implementation of run()
class B implements A {
    public void run() {}
}

// Create a class named MyThread and extend/implement the required class/interface
class MyThread extends B {
    // Define a method in MyThread class to print the output
    @Override
    public void run() {
        System.out.println("NPTEL Java");
    }
}

// Main class W06_P3 is defined
public class W06_P3 {
    public static void main(String[] args) {
        // An object of MyThread class is created
        MyThread t = new MyThread();
        // run() of class MyThread is called
        t.run();
    }
}
```

4. 

```
class Execute {
    synchronized void print(int n) { 
        for (int i = 1; i <= 5; i++) {
            System.out.println(n * i);
            try {
                Thread.sleep(400);
            } catch (Exception e) {
                System.out.println(e);
            }
        }
    }
} 

class Thread1 extends Thread {
    Execute t;
    Thread1(Execute t) {
        this.t = t;
    }
    public void run() {
        t.print(5);
    }
}

class Thread2 extends Thread {
    Execute t;
    Thread2(Execute t) {
        this.t = t;
    }
    public void run() {
        t.print(100);
    }
}

public class W06_P4 {
    public static void main(String args[]) {
        Execute obj = new Execute(); // Only one object  
        Thread1 t1 = new Thread1(obj);
        Thread2 t2 = new Thread2(obj);
        t1.start();
        t2.start();
    }
}

```
---

5. **Add necessary codes to print the following:**



-----------------OUTPUT-------------------

Name of thread 't':Thread-0

New name of thread 't':NPTEL

Thread is running.

-------------------------------------------------
```
class W06_P5 extends Thread {  
    public void run() {  
        System.out.println("Thread is running.");  
    }  
  
    public static void main(String args[]) {  
        W06_P5 t = new W06_P5();  
        
        System.out.println("Name of thread 't':" + t.getName());  
        
        
        t.start();  
        
      
        t.setName("NPTEL");  
        
        System.out.println("New name of thread 't':" + t.getName());  
    }  
}
