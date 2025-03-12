## **Week 7:   Programming In Java**


1. **What will be the output of the following Java program?**  

```java
import java.io.*;  
class ReadFile {  
    public static void main(String[] args) throws IOException {  
        FileReader fr = new FileReader("NPTEL.txt");  
        BufferedReader br = new BufferedReader(fr);  
        System.out.println(br.readLine());  
        br.close();  
    }  
}  
```  
a. Hello, World!  
b. This is Programming in Java online course.  
c. IOException  
d. null  

**Answer:** b. This is Programming in Java online course. 

---

2. **Which of these classes is used to write primitive data types to an output stream in Java?**  

a. FileWriter
b. DataOutputStream  
c. PrintWriter
d. BufferedOutputStream  

**Answer:** b. DataOutputStream  

---

3. **What will the following code print?**  

```java
import java.io.*;

class RandomAccessFileExample {
    public static void main(String[] args) throws IOException {
        RandomAccessFile file = new RandomAccessFile("test.dat", "rw");
        file.writeInt(100);
        file.seek(0);
        System.out.println(file.readInt());
        file.close();
    }
}
```

a. 0  
b. Runtime Error  
c. Compilation Error  
d. 100  

**Answer:** d. 100

---
4. **Complete the following snippet with the required code.**  

```java
File file = new File("file.txt");
if (_________________)  // Fill in the blanks
{
    System.out.println("File exists.");
} 
else 
{
    System.out.println("File does not exist.");
}
```

a. `file.exists()`  
b. `file.isFile()`  
c. `file.fileExists()`  
d. `file.isAvailable()`  

**Answer:** a. `file.exists()`

---

5. **What will the following Java program output?**  

```java
import java.io.*;

class SequenceInputStreamExample {
    public static void main(String[] args) throws IOException {
        ByteArrayInputStream input1 = new ByteArrayInputStream("123".getBytes());
        ByteArrayInputStream input2 = new ByteArrayInputStream("ABC".getBytes());
        SequenceInputStream sequence = new SequenceInputStream(input1, input2);

        int i;
        while ((i = sequence.read()) != -1) {
            System.out.print((char) i);
        }
    }
}
```

a. `123ABC`  
b. `ABC123`  
c. Compilation Error  
d. Runtime Error  

**Answer:** a. `123ABC`  

---

6. Here is the extracted text from the image:

---

**What is the output of the following Java program?**  

```java
class Main {
    public static void main(String args[]) {
        final int i;
        i = 20;
        i = 30;
        System.out.println(i);
    }
}
```

a. `30`  
b. Compiler Error  
c. Garbage value  
d. `0`  

**Answer:** b. Compiler Error

---

7. **What will be the output of the following Java program?**  

```java
import java.io.*;
class Chararrayinput {
    public static void main(String[] args) {
        String obj = "abcdefgh";
        int length = obj.length();
        char c[] = new char[length];
        obj.getChars(0, length, c, 0);
        CharArrayReader input1 = new CharArrayReader(c);
        CharArrayReader input2 = new CharArrayReader(c, 1, 4);
        int i, j;
        try {
            while ((i = input1.read()) == (j = input2.read())) {
                System.out.print((char) i);
            }
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
}
```
  
a. `abc`  
b. `abcd`  
c. `abcde`  
d. `none of the mentioned`  

**Answer:** a. `abc` 

---

8. **What will be the output of the following Java program?**  

```java
public class Calculator {
    int num = 100;

    public void calc(int num) {
        this.num = num * 10;
    }

    public void printNum() {
        System.out.println(num);
    }

    public static void main(String[] args) {
        Calculator obj = new Calculator();
        obj.calc(2);
        obj.printNum();
    }
}
```

a. `20`  
b. `100`  
c. `1000`  
d. `2`  

**Answer:** c. `1000`  

---

9. **What will be the output of the following code?**

```java
import java.io.*;

public class W7 {
    public static void main(String[] args) {
        try {
            PrintWriter writer = new PrintWriter(System.out);

            writer.write(9 + 97);

            writer.close();
        } catch (Exception e) {
            System.out.println(e);
        }
    }
}
```

a. It will give compile-time error  
b. It will give run-time error  
c. `j`  
d. `106`  

**Answer:** c. `j`

---

10. **What will be the output of the following code?**  
**file.txt contains:**  
*"This is Programming in Java online course."* (without quotes)  

```java
import java.io.File;

class FileSizeExample {
    public static void main(String[] args) {
        // Specify the file path
        String filePath = "file.txt";

        // Create a File object
        File file = new File(filePath);

        // Get the size of the file
        long fileSize = file.length();

        // Print the size of the file
        System.out.println(fileSize);
    }
}
```

a. 42  
b. 35  
c. 7  
d. 0  

**Answer:** a. 42

---
