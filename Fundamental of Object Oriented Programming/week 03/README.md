# **Week 3 Assignment 3 - Fundamentals of Object-Oriented Programming**

## **Questions and Answers**

### **1. Consider the following code:**

class A {
public:
    void display() { std::cout << "Base class A\n"; }
};

class B : public A {
public:
    void show() { std::cout << "Derived class B\n"; }
};

int main() {
    B obj;
    obj.display();
    obj.show();
    return 0;
}

**What is the output of the above program?**

- **a)** Base class A  
  Derived class B  
- **b)** Derived class B  
  Base class A  
- **c)** Base class A  
- **d)** Derived class B  

**Answer:** a) Base class A  
   Derived class B  

---

### **2. In C++, ambiguity occurs in multiple inheritance when:**

- **a)** A derived class has a method with the same name as a method in the base class.  
- **b)** Two base classes have methods with the same name, and a derived class inherits from both.  
- **c)** A derived class has no constructor defined.  
- **d)** A base class has a private member function.  

**Answer:** b) Two base classes have methods with the same name, and a derived class inherits from both.  

---

### **3. Which of the following correctly calls all three methods from an object of C in multilevel inheritance?**

- **a)** C obj; obj.display(); obj.show(); obj.output();`  
- **b)** B obj; obj.show(); obj.output();`  
- **c)** A obj; obj.display(); obj.show(); obj.output();`  
- **d)** C obj; obj.output();`  

**Answer:** a) `C obj; obj.display(); obj.show(); obj.output();`  

---

### **4. Consider the following Java code:**

class A {
    void display() { System.out.println("Class A"); }
}

class B extends A {
    void show() { System.out.println("Class B"); }
}

class C extends A {
    void output() { System.out.println("Class C"); }
}

public class Main {
    public static void main(String[] args) {
        B objB = new B();
        objB.display(); 
        objB.show();
        C objC = new C();
        objC.display(); 
        objC.output();
    }
}

**What is the output of the above program?**

- **a)** Class A  
  Class B  
  Class A  
  Class C  
- **b)** Class B  
  Class A  
  Class C  
- **c)** Class A  
  Class A  
- **d)** Class B  
  Class C  

**Answer:** a) Class A  
   Class B  
   Class A  
   Class C  

---

### **5. Which of the following is true about method overriding in Java?**

- **a)** The overridden method must have a different return type.  
- **b)** The overridden method must have the same name and parameters as the base class method.  
- **c)** The base class method must be private.  
- **d)** Overriding is not possible in Java.  

**Answer:** b) The overridden method must have the same name and parameters as the base class method.  

---

### **6. Consider the following C++ code:**
```cpp
class Base {
public:
    virtual void display() { std::cout << "Base class\n"; }
};

class Derived : public Base {
public:
    void display() override { std::cout << "Derived class\n"; }
};

int main() {
    Base* ptr;
    Derived obj;
    ptr = &obj;
    ptr->display();
    return 0;
}
```
**What is the output of the program?**

- **a)** Base class  
- **b)** Derived class  
- **c)** Compilation error  
- **d)** Undefined behavior  

**Answer:** b) Derived class  

---

### **7. Which of the following statements about virtual functions is false?**

- **a)** Virtual functions allow dynamic (runtime) polymorphism.  
- **b)** A virtual function must be declared as virtual in the base class.  
- **c)** A virtual function can have default arguments.  
- **d)** A virtual function cannot be overridden in a derived class.  

**Answer:** d) A virtual function cannot be overridden in a derived class.  

---

### **8. Which of the following correctly uses a base class pointer to call `area()` for both shapes in a C++ virtual function program?**

- **a)** `Shape* ptr; Rectangle rect; ptr = &rect; ptr->area();`  
- **b)** `Shape* ptr = new Circle(r); ptr->area();`  
- **c)** Both a and b  
- **d)** None of the above  

**Answer:** a) `Shape* ptr; Rectangle rect; ptr = &rect; ptr->area();`  

---

### **9. How are public and protected members of the base class treated in the derived class when using protected inheritance?**

- **a)** They both become private members in the derived class.  
- **b)** They both remain public members in the derived class.  
- **c)** They both become protected members in the derived class.  
- **d)** They are inaccessible in the derived class.  

**Answer:** c) They both become protected members in the derived class.  

---

### **10. Which of the following is a potential problem associated with multiple inheritance in C++?**

- **a)** Ambiguity in accessing members when two base classes have members with the same name.  
- **b)** Lack of runtime polymorphism.  
- **c)** Inability to overload operators in derived classes.  
- **d)** Restriction on the number of base classes a derived class can inherit from.  

**Answer:** a) Ambiguity in accessing members when two base classes have members with the same name.  
