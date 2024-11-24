
# Java Programming Concepts

## **Basics**

### **1. Introduction to Java**
#### Program: Hello, World!
```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```

---

### **2. Variables and Data Types**
#### Program: Variable Declaration and Initialization
```java
public class VariablesDemo {
    public static void main(String[] args) {
        int age = 25;
        double price = 99.99;
        char grade = 'A';
        String name = "John";
        boolean isJavaFun = true;

        System.out.println("Age: " + age);
        System.out.println("Price: $" + price);
        System.out.println("Grade: " + grade);
        System.out.println("Name: " + name);
        System.out.println("Is Java Fun? " + isJavaFun);
    }
}
```

---

### **3. Conditional Statements**
#### Program: Check if a Number is Even or Odd
```java
public class EvenOddCheck {
    public static void main(String[] args) {
        int number = 7;
        if (number % 2 == 0) {
            System.out.println(number + " is even.");
        } else {
            System.out.println(number + " is odd.");
        }
    }
}
```

---

### **4. Loops**
#### Program: Sum of Numbers from 1 to 10
```java
public class SumNumbers {
    public static void main(String[] args) {
        int sum = 0;
        for (int i = 1; i <= 10; i++) {
            sum += i;
        }
        System.out.println("Sum: " + sum);
    }
}
```

---

## **Intermediate**

### **1. Classes and Objects**
#### Program: Create and Use a Simple Class
```java
class Student {
    String name;
    int age;

    void displayInfo() {
        System.out.println("Name: " + name);
        System.out.println("Age: " + age);
    }
}

public class StudentDemo {
    public static void main(String[] args) {
        Student student = new Student();
        student.name = "Alice";
        student.age = 20;
        student.displayInfo();
    }
}
```

---

### **2. Arrays**
#### Program: Reverse an Array
```java
public class ReverseArray {
    public static void main(String[] args) {
        int[] numbers = {1, 2, 3, 4, 5};
        System.out.print("Reversed Array: ");
        for (int i = numbers.length - 1; i >= 0; i--) {
            System.out.print(numbers[i] + " ");
        }
    }
}
```

---

### **3. Methods**
#### Program: Calculate Factorial Using a Method
```java
public class Factorial {
    public static int factorial(int n) {
        if (n == 0 || n == 1) return 1;
        return n * factorial(n - 1);
    }

    public static void main(String[] args) {
        int num = 5;
        System.out.println("Factorial of " + num + " is " + factorial(num));
    }
}
```

---

### **4. Inheritance**
#### Program: Demonstrate Inheritance
```java
class Animal {
    void eat() {
        System.out.println("This animal eats food.");
    }
}

class Dog extends Animal {
    void bark() {
        System.out.println("The dog barks.");
    }
}

public class InheritanceDemo {
    public static void main(String[] args) {
        Dog dog = new Dog();
        dog.eat();
        dog.bark();
    }
}
```

---

## **Advanced**

### **1. Polymorphism**
#### Program: Method Overloading
```java
class Calculator {
    int add(int a, int b) {
        return a + b;
    }

    double add(double a, double b) {
        return a + b;
    }
}

public class PolymorphismDemo {
    public static void main(String[] args) {
        Calculator calc = new Calculator();
        System.out.println("Sum (int): " + calc.add(5, 10));
        System.out.println("Sum (double): " + calc.add(5.5, 10.5));
    }
}
```

---

### **2. Exception Handling**
#### Program: Handle Division by Zero
```java
public class ExceptionHandling {
    public static void main(String[] args) {
        try {
            int result = 10 / 0;
            System.out.println("Result: " + result);
        } catch (ArithmeticException e) {
            System.out.println("Error: Division by zero is not allowed.");
        }
    }
}
```

---

### **3. Collections**
#### Program: Using ArrayList
```java
import java.util.ArrayList;

public class ArrayListDemo {
    public static void main(String[] args) {
        ArrayList<String> fruits = new ArrayList<>();
        fruits.add("Apple");
        fruits.add("Banana");
        fruits.add("Cherry");

        System.out.println("Fruits: " + fruits);

        fruits.remove("Banana");
        System.out.println("Updated Fruits: " + fruits);
    }
}
```

---

### **4. File Handling**
#### Program: Writing to a File
```java
import java.io.FileWriter;
import java.io.IOException;

public class FileWriteDemo {
    public static void main(String[] args) {
        try {
            FileWriter writer = new FileWriter("output.txt");
            writer.write("Hello, World! This is written to a file.");
            writer.close();
            System.out.println("File written successfully.");
        } catch (IOException e) {
            System.out.println("An error occurred: " + e.getMessage());
        }
    }
}
```
