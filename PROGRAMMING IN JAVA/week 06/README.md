## **Week 6:  Programming In Java**

#### **1. Consider the following code snippet:**  

```java
class MyThread extends Thread {
    public void run() {
        for (int i = 0; i < 3; i++) {
            System.out.println("Running thread: " + i);
        }
    }
}

public class Main {
    public static void main(String[] args) {
        MyThread thread = new MyThread();
        thread.run();
        System.out.println("Main method complete.");
    }
}
```
**What will be the output of the program?**  

**a.**  
```
Running thread: 0  
Running thread: 1  
Running thread: 2  
Main method complete.
```

**b.**  
```
Running thread: 0  
Main method complete.  
Running thread: 1  
Running thread: 2
```

**c.**  
```
Main method complete.
```

**d.**  
```
Error: The thread was not started using start()
```


**Answer:** a

---

#### **2. Which of the following best describes the concept of multithreading in Java?**  

**a.** Multiple threads execute concurrently, sharing the same memory space.  
**b.** Only one thread executes at a time, ensuring sequential execution.  
**c.** Threads in Java cannot communicate with each other.  
**d.** Threads require separate memory allocation for each thread to run.  

**Answer:** a 

---

#### **3. What will happen when the following code is executed?**  

```java
class ExampleThread extends Thread {
    public void run() {
        System.out.println("Thread is running.");
    }
}

public class Main {
    public static void main(String[] args) {
        ExampleThread thread = new ExampleThread();
        thread.start();
        thread.start();
    }
}
```
**a.** The program will execute successfully, printing "Thread is running." twice.  
**b.** The program will throw an error when attempting to start the thread a second time.  
**c.** The program will terminate without any output.  
**d.** The thread will run only once, and the second `start()` call will be ignored.  

**Answer:** b  

---

#### **4. Find the error in the following program:**  

```java
class RunnableExample implements Runnable {
    public void run() {
        for (int i = 1; i <= 3; i++) {
            System.out.println("Runnable thread: " + i);
        }
    }
}

public class Main {
    public static void main(String[] args) {
        RunnableExample runnable = new RunnableExample();
        runnable.run();
        System.out.println("Main method ends.");
    }
}
```

**a.** The program will throw an error because Runnable cannot be executed directly.  
**b.** The program will run successfully but will not create a new thread.  
**c.** The program will create a new thread and execute concurrently.  
**d.** The program will throw a runtime error because Thread is not used.  

**Answer:** b

---

#### **5. What will happen when the following code is executed?**

```java
class RunnableExample implements Runnable {
    public void run() {
        for (int i = 1; i <= 3; i++) {
            System.out.println("Thread running: " + i);
        }
    }
}

public class Main {
    public static void main(String[] args) {
        RunnableExample task = new RunnableExample();
        Thread thread = new Thread(task);
        thread.start();
    }
}
```
**a.** The program will throw a compile-time error because `Runnable` is not a thread.  
**b.** The program will execute successfully, and the `run()` method will run in a new thread.  
**c.** The program will execute the `run()` method directly on the main thread.  
**d.** The program will throw a runtime error because `Runnable` is not properly implemented.  

**Answer:** b  

---

#### **6. Which of the following states can a thread enter during its lifecycle in Java?**  

a. **New, Runnable, Running, Blocked**  
b. **New, Runnable, Waiting, Blocked, Terminated**  
c. **New, Runnable, Running, Sleeping, Dead**  
d. **New, Active, Waiting, Suspended, Terminated**  

**Answer:** b
 
---

#### **7. What does the thread scheduler use to decide which thread to run when multiple threads are in the runnable state?**  

a. **Thread priority**  
b. **Thread's execution time**  
c. **Thread name**  
d. **Thread creation order**  

**Answer:** a

---

#### **8. Consider the following program:**  

```java
class PriorityExample extends Thread {  
    public void run() {  
        System.out.println(Thread.currentThread().getName() +  
                           " with priority " +  
                           Thread.currentThread().getPriority());  
    }  
}  

public class Main {  
    public static void main(String[] args) {  
        PriorityExample t1 = new PriorityExample();  
        PriorityExample t2 = new PriorityExample();  
        
        t1.setPriority(Thread.MIN_PRIORITY);  
        t2.setPriority(Thread.MAX_PRIORITY);  
        
        t1.start();  
        t2.start();  
    }  
}
```

---

**Which of the following is true about the output?**  

a. **The thread with the higher priority is guaranteed to execute first.**  
b. **The thread with the lower priority will never execute.**  
c. **The order of execution depends on the JVM and OS scheduling policies.**  
d. **The program will throw an error due to invalid priority values.**  

**Answer:** c

---
#### **9. What is the primary purpose of thread synchronization in Java?**  

a. **To allow multiple threads to execute a method at the same time**  
b. **To ensure thread execution follows a specific order**  
c. **To prevent race conditions and ensure data consistency**  
d. **To allow threads to communicate with each other**  

**Answer:** c  

---

#### **10. What is the primary difference between Byte Streams and Character Streams in Java?**  

a. **Byte Streams handle characters, while Character Streams handle bytes.**  
b. **Byte Streams are used for binary data, while Character Streams are used for text data.**  
c. **Character Streams are faster than Byte Streams in all cases.**  
d. **Character Streams cannot handle international characters like Unicode.**  

**Answer:** b  
  
---
