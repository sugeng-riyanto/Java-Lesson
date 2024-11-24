
# Lesson 1: Introduction to Java Programming

## **Objective**
By the end of this lesson, students will:
- Understand what Java is and why it's widely used.
- Set up the Java development environment.
- Write and run their first Java program.

---

## **1. What is Java?**
- **Definition**: Java is a high-level, object-oriented programming language that is platform-independent.
- **Features**:
  - Platform independence via Java Virtual Machine (JVM).
  - Widely used in web development, mobile apps (Android), and enterprise solutions.
  - Easy to learn for beginners and powerful for advanced programmers.

---

## **2. Why Learn Java?**
- Cross-platform support.
- Object-oriented design makes programs modular and reusable.
- Strong community and job opportunities.

---

## **3. Java Environment Setup**
### **Steps**:
1. **Download and Install JDK**:
   - Go to [Oracle JDK](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html) or use OpenJDK.
   - Install the JDK on your system.
2. **Set up an IDE**:
   - Install IntelliJ IDEA, Eclipse, or VS Code.
   - Configure the IDE to use the JDK.

### **Activity**:
- Verify installation:
  - Open the terminal/command prompt.
  - Type `java --version` and `javac --version` to check if Java is installed.

---

## **4. Your First Java Program**
### **Code**:
```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```

### **Steps to Run**:
1. Open the IDE and create a new Java project.
2. Create a file named `HelloWorld.java`.
3. Copy and paste the code into the file.
4. Compile and run the program:
   - In the terminal: `javac HelloWorld.java` and then `java HelloWorld`.
   - In the IDE: Click the **Run** button.

---

## **5. Key Concepts in the Program**
1. **Class**: `HelloWorld` is the class name. It must match the filename.
2. **Method**: `main()` is the entry point of the program.
3. **Statement**: `System.out.println("Hello, World!");` prints text to the console.

---

## **6. Activity**
### **Objective**:
Write a program that prints your name and favorite programming language.

### **Example**:
```java
public class AboutMe {
    public static void main(String[] args) {
        System.out.println("My name is John.");
        System.out.println("My favorite programming language is Java.");
    }
}
```

---

## **7. Homework**
1. Research the difference between JVM, JRE, and JDK.
2. Install an IDE if not already done and write a program that prints:
   - Your name.
   - Your hobby.

---

## **Conclusion**
- Java is a powerful, beginner-friendly programming language.
- You successfully wrote and ran your first Java program.
- Next Lesson: **Java Basics** (data types, variables, and control structures).

---

### **References**
- [Oracle Java Documentation](https://docs.oracle.com/en/java/)
- [Java Installation Guide](https://www.oracle.com/java/technologies/javase-downloads.html)
