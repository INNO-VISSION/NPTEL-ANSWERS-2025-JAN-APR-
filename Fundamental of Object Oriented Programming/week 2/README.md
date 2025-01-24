### Week 2: Assignment 2 - Fundamentals of Object-Oriented Programming  

### Questions and Answers  

1. *Which of the following best describes a class in object-oriented programming?*  
   Options:  
   - a. A block of code that defines functions only.  
   - b. A blueprint for creating objects, encapsulating data and methods.  
   - c. A template for functions without data.  
   - d. A data structure for storing primitive data types.  
   *Answer*: b. A blueprint for creating objects, encapsulating data and methods.  

2. *What happens when an object is created from a class in C++?*  
   Options:  
   - a. Memory is allocated for the object’s member variables only.  
   - b. Memory is allocated for member functions and variables.  
   - c. Member functions are inherited, and memory is allocated for them.  
   - d. Member functions are shared across objects, and memory is allocated only for variables.  
   *Answer*: b. Memory is allocated for member functions and variables.  

3. *Which of the following statements about constructors is false?*  
   Options:  
   - a. Constructors must have the same name as the class.  
   - b. Constructors can be overloaded in C++.  
   - c. Constructors cannot be private in C++.  
   - d. Constructors do not have a return type.  
   *Answer*: c. Constructors cannot be private in C++.  

4. *In Java, the proper way to define a class Circle with:*  
   Options:  
   - a. A constructor that initializes its radius.  
   - b. A method area() to return the area of the circle.  
   Options:  
   - a. Circle c1 = Circle(radius);  
   - b. Circle c1 = new Circle(radius);  
   - c. Circle c1 = new Circle.radius();  
   *Answer*: b. Circle c1 = new Circle(radius);  

5. *Consider the following C++ code:*  
   
   #include <iostream>
   
   class Test {
   
   public:
   
       Test() { std::cout << "Constructor called\n"; }
       ~Test() { std::cout << "Destructor called\n"; }
       void display() { std::cout << "Display function\n"; }
   };
   
   int main() {
   
       Test t1;
       t1.display();
       return 0;
   }
     
   What is the output of this program?  
   Options:  
   - a. Constructor called  
      Display function  
      Destructor called  
   - b. Constructor called  
      Destructor called  
      Display function  
   - c. Display function  
      Constructor called  
      Destructor called  
   - d. Constructor called  
      Display function  
   *Answer*: a. Constructor called  
               Display function  
               Destructor called  

6. *What is the primary purpose of a destructor in C++?*  
   Options:  
   - a. To initialize an object when it is created.  
   - b. To release memory and resources when an object is destroyed.  
   - c. To overload operators for memory allocation.  
   - d. To define default behavior for inheritance.  
   *Answer*: b. To release memory and resources when an object is destroyed.  

7. *Consider the following C++ code:*  
   
   #include <iostream>
   
   class Sample {
   
   public:
   
       Sample() { std::cout << "Constructor called\n"; }
       ~Sample() { std::cout << "Destructor called\n"; }
   
   };
   
   void createObject() {
   
       Sample obj;
       std::cout << "Inside createObject function\n";
   }
   
   int main() {
   
       std::cout << "Before calling createObject\n";
       createObject();
       std::cout << "After calling createObject\n";
       return 0;
   }
     
   What is the output of this program?  
   Options:  
   - a. Constructor called  
         Inside createObject function  
         Destructor called  
   - b. Before calling createObject  
         After calling createObject  
   - c. Before calling createObject  
         Constructor called  
         Inside createObject function  
         Destructor called  
         After calling createObject  
   - d. Inside createObject function  
         Constructor called  
         After calling createObject  
   *Answer*: c. Before calling createObject  
                  Constructor called  
                  Inside createObject function  
                  Destructor called  
                  After calling createObject  

8. *A class in C++ has multiple constructors. How does the compiler decide which constructor to use?*  
   Options:  
   - a. Based on the return type.  
   - b. Based on the arguments passed during object creation.  
   - c. The first constructor is always used.  
   - d. The last constructor is always used.  
   *Answer*: b. Based on the arguments passed during object creation.  

9. *In a C++ program that:*  
   - Defines a class FileHandler with a constructor that opens a file and a destructor that closes the file.  
   - Demonstrates file handling using objects of this class.  
   Choose the correct constructor signature:  
   Options:  
   - a. FileHandler(std::string filename);  
   - b. FileHandler(char* filename);  
   - c. FileHandler(const char filename[]);  
   - d. All of the above  
   *Answer*: d. All of the above  

10. *Analyze the following C++ code and identify the correct output:*  
    
    #include <iostream>
    
    class Rectangle {
    
        int length, width;
    
    public:
    
        Rectangle(int l, int w) : length(l), width(w) {}
        int area() { return length * width; }
    };
    
    int main() {
    
        Rectangle rect(5, 3);
        std::cout << rect.area();
        return 0;
    }
      
    Options:  
    - a. 15  
    - b. 8  
    - c. Compilation error  
    - d. Undefined behavior  
    *Answer*: a. 15
