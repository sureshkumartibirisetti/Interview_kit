

# 💻 Core Java Topics - From Basic to Advanced

---

### ✅ 1. Java Basics
- Java is a high-level, object-oriented, class-based programming language.
- **Platform Independent**: Java programs are compiled into bytecode by the Java Compiler, which runs on any system with a Java Virtual Machine (JVM).
- **WORA**: Write Once, Run Anywhere.

---

### 🧱 2. Hello Java Program
```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, Java!");
    }
}
```

---

### 🧠 3. Internal Details of JVM
- **JVM**: Java Virtual Machine — executes Java bytecode.
- **JRE**: Java Runtime Environment — JVM + libraries.
- **JDK**: Java Development Kit — JRE + tools (compiler, debugger).
- Components: Class Loader, Bytecode Verifier, Execution Engine

---

### 📦 4. Packages
```java
package mypackage;
import java.util.Scanner;
```
- Helps avoid name conflicts and controls access.

---

### 🔐 5. Access Modifiers
| Modifier   | Class | Package | Subclass | World |
|------------|-------|---------|----------|--------|
| `public`     | ✅     | ✅       | ✅        | ✅      |
| `protected`  | ✅     | ✅       | ✅        | ❌      |
| `default`    | ✅     | ✅       | ❌        | ❌      |
| `private`    | ✅     | ❌       | ❌        | ❌      |

---

### 👥 6. Class vs Object
- **Class**: Template/blueprint for objects.
- **Object**: Instance of a class.

```java
class Car {
    int speed;
    void drive() { System.out.println("Driving"); }
}
Car myCar = new Car();
```

---

### 🧱 7. Constructor in Java
- Special method to initialize objects.
- Same name as class, no return type.

```java
public Car() {
   speed = 50;
}
```

---

### 🔁 8. Java Methods
- Block of code that performs a specific task.

```java
int add(int a, int b) {
   return a + b;
}
```

---

### 🧰 9. Reference Variables
- Stores the reference (memory address) of an object.

```java
Car car1 = new Car();
```

---

### 🎯 10. Data Types
- **Primitive**: byte, short, int, long, float, double, char, boolean
- **Non-Primitive**: String, Arrays, Objects

---

### 💡 11. Java OOPs Concepts
- **Encapsulation**: Hiding internal details
- **Inheritance**: Reusing code from a parent class
- **Polymorphism**: Many forms (overloading & overriding)
- **Abstraction**: Hiding implementation using abstract class or interface

---

### 🔍 12. Inheritance
```java
class Animal {
    void eat() {}
}
class Dog extends Animal {
    void bark() {}
}
```

---

### 🎭 13. Overloading and Overriding
- **Overloading**: Same method name, different parameters
```java
void show(int a) {}
void show(String b) {}
```
- **Overriding**: Redefining a parent class method in child class

---

### 🔐 14. Final Keyword
- `final` variable: Constant
- `final` method: Cannot be overridden
- `final` class: Cannot be extended

---

### 🔁 15. Abstract Classes
```java
abstract class Shape {
    abstract void draw();
}
```

---

### 🔌 16. Interfaces
```java
interface Drawable {
    void draw();
}
```

---

### ⚙️ 17. Exception Handling
```java
try {
   int a = 5 / 0;
} catch (ArithmeticException e) {
   System.out.println("Cannot divide by zero");
} finally {
   System.out.println("Always executes");
}
```

---

### 🧵 18. Multithreading
```java
class MyThread extends Thread {
    public void run() {
        System.out.println("Thread running");
    }
}
```

---

### 🗃️ 19. Java Arrays
```java
int[] arr = new int[5];
```

---

### 🗂️ 20. Collections vs Collection Framework
- **Collection**: Interface (List, Set)
- **Collections**: Utility class with methods like `sort()`, `reverse()`
- **Collection Framework**: Architecture for manipulating group of objects

---

### 📚 21. Collections
- **List**: Ordered, allows duplicates (`ArrayList`, `LinkedList`)
- **Set**: No duplicates (`HashSet`, `TreeSet`)
- **Queue**: FIFO (`PriorityQueue`, `LinkedList`)

---

### 🧰 22. Java Map
```java
Map<String, Integer> map = new HashMap<>();
map.put("A", 1);
System.out.println(map.get("A")); // Output: 1
```

---

### 🧪 23. Generic Methods
```java
public <T> void print(T data) {
   System.out.println(data);
}
```
