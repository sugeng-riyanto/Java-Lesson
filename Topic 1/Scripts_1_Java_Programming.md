
# Lesson 1: Java Programming - Writing and Running Your First Program

## **Step-by-Step Guide**

### **Step 1: Install Java Development Kit (JDK)**
1. Download the JDK from [Oracle JDK](https://www.oracle.com/java/technologies/javase-downloads.html) or use OpenJDK.
2. Install the JDK on your system.
3. Verify installation:
   - Open a terminal or command prompt.
   - Type: `java --version` to check the installed Java version.

---

### **Step 2: Set Up an IDE**
#### Recommended IDEs:
- **IntelliJ IDEA** (Beginner-friendly, robust).
- **Eclipse** (Widely used in enterprises).
- **VS Code** (Lightweight with Java extensions).

#### **Steps to Set Up IntelliJ IDEA**:
1. Download and install IntelliJ IDEA from [JetBrains](https://www.jetbrains.com/idea/).
2. Open IntelliJ and configure it to use the installed JDK.
   - Go to **File → Project Structure → SDK**.
   - Select the JDK path (usually located in `C:\Program Files\Java\jdk-xx.x.x`).

---

### **Step 3: Write the Code**
#### Example Code: `HelloWorld.java`
```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```

#### Steps:
1. Open your IDE.
2. Create a new **Java Project**.
3. Inside the project, create a new file:
   - File name: `HelloWorld.java`
   - File type: Java Class.
4. Copy the code above into the file.

---

### **Step 4: Run the Program**
#### Using IntelliJ IDEA:
1. Save the file.
2. Click the **Run** button or right-click on the file and select **Run HelloWorld**.
3. View the output in the console at the bottom of the IDE:
   ```
   Hello, World!
   ```

#### Using Command Line (Optional):
1. Open a terminal or command prompt.
2. Navigate to the folder containing `HelloWorld.java`.
3. Compile the program:
   ```
   javac HelloWorld.java
   ```
4. Run the program:
   ```
   java HelloWorld
   ```
5. The output will be:
   ```
   Hello, World!
   ```

---

### **Step 5: Modify and Experiment**
Encourage students to modify the code and try:
1. Printing their name:
   ```java
   System.out.println("My name is John.");
   ```
2. Adding more messages:
   ```java
   System.out.println("I am learning Java programming!");
   ```

---

### **Step 6: Homework**
1. Research what each part of the program does:
   - `public class`: Definition of the class.
   - `public static void main(String[] args)`: The entry point of the Java program.
   - `System.out.println`: Command to print text.
2. Create a program to display:
   - Your name.
   - Your favorite hobby.
   - Your goal for learning Java.

---

### **Example Extended Program**
```java
public class AboutMe {
    public static void main(String[] args) {
        System.out.println("My name is Sarah.");
        System.out.println("My favorite hobby is painting.");
        System.out.println("My goal is to become a Java developer.");
    }
}
```
