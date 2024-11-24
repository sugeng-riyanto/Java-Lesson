
# Java Programming Concepts with Line-by-Line Comments

## **Basics**

### **1. Introduction to Java**
#### Program: Hello, World!
```java
// Define the main class
public class HelloWorld {
    // Entry point of the program
    public static void main(String[] args) {
        // Print "Hello, World!" to the console
        System.out.println("Hello, World!");
    }
}
```

---

### **2. Variables and Data Types**
#### Program: Variable Declaration and Initialization
```java
// Demonstrating variables of different data types
public class VariablesDemo {
    public static void main(String[] args) {
        // Integer variable to store age
        int age = 25;

        // Double variable to store a price
        double price = 99.99;

        // Character variable to store a grade
        char grade = 'A';

        // String variable to store a name
        String name = "John";

        // Boolean variable to indicate if Java is fun
        boolean isJavaFun = true;

        // Print all the variables
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
// Check if a number is even or odd
public class EvenOddCheck {
    public static void main(String[] args) {
        // Number to check
        int number = 7;

        // Check if the number is divisible by 2
        if (number % 2 == 0) {
            // If true, print that the number is even
            System.out.println(number + " is even.");
        } else {
            // If false, print that the number is odd
            System.out.println(number + " is odd.");
        }
    }
}
```

---

### **4. Loops**
#### Program: Sum of Numbers from 1 to 10
```java
// Calculate the sum of numbers from 1 to 10 using a loop
public class SumNumbers {
    public static void main(String[] args) {
        // Variable to store the sum
        int sum = 0;

        // Loop through numbers 1 to 10
        for (int i = 1; i <= 10; i++) {
            // Add the current number to the sum
            sum += i;
        }

        // Print the total sum
        System.out.println("Sum: " + sum);
    }
}
```

---

## **Intermediate**

### **1. Classes and Objects**
#### Program: Create and Use a Simple Class
```java
// Define a class named Student
class Student {
    // Attributes of the Student class
    String name;
    int age;

    // Method to display student information
    void displayInfo() {
        System.out.println("Name: " + name);
        System.out.println("Age: " + age);
    }
}

// Main class to demonstrate objects
public class StudentDemo {
    public static void main(String[] args) {
        // Create an object of the Student class
        Student student = new Student();

        // Assign values to the object's attributes
        student.name = "Alice";
        student.age = 20;

        // Call the method to display student information
        student.displayInfo();
    }
}
```

---

### **2. Arrays**
#### Program: Reverse an Array
```java
// Reverse the elements of an array
public class ReverseArray {
    public static void main(String[] args) {
        // Initialize an array with numbers
        int[] numbers = {1, 2, 3, 4, 5};

        // Print the reversed array
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
// Calculate the factorial of a number using recursion
public class Factorial {
    // Method to calculate factorial
    public static int factorial(int n) {
        // Base case: factorial of 0 or 1 is 1
        if (n == 0 || n == 1) return 1;

        // Recursive case: n * factorial of (n-1)
        return n * factorial(n - 1);
    }

    public static void main(String[] args) {
        // Number to calculate factorial for
        int num = 5;

        // Print the factorial of the number
        System.out.println("Factorial of " + num + " is " + factorial(num));
    }
}
```

---

### **4. Inheritance**
#### Program: Demonstrate Inheritance
```java
// Define a parent class named Animal
class Animal {
    // Method in the parent class
    void eat() {
        System.out.println("This animal eats food.");
    }
}

// Define a child class named Dog that extends Animal
class Dog extends Animal {
    // Method specific to the Dog class
    void bark() {
        System.out.println("The dog barks.");
    }
}

// Main class to demonstrate inheritance
public class InheritanceDemo {
    public static void main(String[] args) {
        // Create an object of the Dog class
        Dog dog = new Dog();

        // Call the parent class method
        dog.eat();

        // Call the child class method
        dog.bark();
    }
}
```

---

## **Advanced**

### **1. Polymorphism**
#### Program: Method Overloading
```java
// Demonstrate method overloading
class Calculator {
    // Method to add two integers
    int add(int a, int b) {
        return a + b;
    }

    // Method to add two doubles
    double add(double a, double b) {
        return a + b;
    }
}

// Main class to demonstrate polymorphism
public class PolymorphismDemo {
    public static void main(String[] args) {
        Calculator calc = new Calculator();

        // Call the integer addition method
        System.out.println("Sum (int): " + calc.add(5, 10));

        // Call the double addition method
        System.out.println("Sum (double): " + calc.add(5.5, 10.5));
    }
}
```

---

### **2. Exception Handling**
#### Program: Handle Division by Zero
```java
// Demonstrate exception handling
public class ExceptionHandling {
    public static void main(String[] args) {
        try {
            // Attempt to divide by zero
            int result = 10 / 0;

            // This line will not be executed due to the exception
            System.out.println("Result: " + result);
        } catch (ArithmeticException e) {
            // Handle the exception
            System.out.println("Error: Division by zero is not allowed.");
        }
    }
}
```

---

### **3. Collections**
#### Program: Using ArrayList
```java
// Demonstrate usage of ArrayList
import java.util.ArrayList;

public class ArrayListDemo {
    public static void main(String[] args) {
        // Create an ArrayList of strings
        ArrayList<String> fruits = new ArrayList<>();

        // Add elements to the ArrayList
        fruits.add("Apple");
        fruits.add("Banana");
        fruits.add("Cherry");

        // Print all elements
        System.out.println("Fruits: " + fruits);

        // Remove an element
        fruits.remove("Banana");

        // Print the updated ArrayList
        System.out.println("Updated Fruits: " + fruits);
    }
}
```

---

### **4. File Handling**
#### Program: Writing to a File
```java
// Write data to a file
import java.io.FileWriter;
import java.io.IOException;

public class FileWriteDemo {
    public static void main(String[] args) {
        try {
            // Create a FileWriter object to write to a file
            FileWriter writer = new FileWriter("output.txt");

            // Write data to the file
            writer.write("Hello, World! This is written to a file.");

            // Close the file writer
            writer.close();

            // Print a success message
            System.out.println("File written successfully.");
        } catch (IOException e) {
            // Handle any exceptions
            System.out.println("An error occurred: " + e.getMessage());
        }
    }
}
```
