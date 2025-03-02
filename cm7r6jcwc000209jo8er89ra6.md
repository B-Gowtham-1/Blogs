---
title: "Day 5: Recap of Java Basics – Everything I’ve Learned So Far!"
seoTitle: "Java Basics Recap: Key Learnings Thus Far"
seoDescription: "Java basics: JDK, JRE, JVM, memory management, I/O, conditionals, loops, functions, arrays, switch statements"
datePublished: Sun Mar 02 2025 05:17:34 GMT+0000 (Coordinated Universal Time)
cuid: cm7r6jcwc000209jo8er89ra6
slug: day-5-recap-of-java-basics-everything-ive-learned-so-far
tags: java, dsa, kunalkushwaha, wemakedevs

---

Alright, today is all about **recapping** what I’ve learned from **Day 1 to Day 4** of my Java journey. It’s time to reflect, refresh, and remind myself that I am slowly but surely becoming a **Java pro** (or at least less confused than before).

---

## **Day 1: Java Basics – Setting the Foundation**

Ah, the day I officially stepped into the **Java world.** Here’s what I learned:

### ☕ **JDK, JRE, and JVM – The Holy Trinity of Java**

* **JDK (Java Development Kit):** The full package – includes everything I need to write, compile, and run Java code.
    
* **JRE (Java Runtime Environment):** Only helps in running Java programs, but can’t compile them.
    
* **JVM (Java Virtual Machine):** The **real MVP**, it runs Java programs by converting them into **bytecode** that computers understand.
    

### 🧠 **Memory Management in Java**

* **Stack Memory:** Stores method calls and local variables (used for fast execution).
    
* **Heap Memory:** Stores objects and dynamic data.
    
* **Garbage Collector:** Automatically deletes unused objects (so I don’t have to clean up my own mess).
    

### 🖥 **Taking Input & Printing Output**

* Used **Scanner** to take input:
    
    ```java
    import java.util.Scanner;
    
    public class InputExample {
        public static void main(String[] args) {
            Scanner sc = new Scanner(System.in);
            System.out.print("Enter your name: ");
            String name = sc.nextLine();
            System.out.println("Hello, " + name + "!");
        }
    }
    ```
    
* Printed output using **System.out.println()** (which I’ve now typed **a million times**).
    

### 🔄 **Conditionals & Loops**

* **if-else statements** to make decisions.
    
* **for loop, while loop, do-while loop** to run code multiple times (aka repeat the pain).
    

---

## **Day 2: Functions and Methods – Reusing Code Like a Pro**

This day was all about writing **functions** (also called **methods**) to avoid writing the same code over and over again.

### **What is a Function?**

A **function** is a block of code that performs a **specific task** and can be reused. It **reduces code repetition** and makes life easier.

### **How to Define a Function in Java?**

```java
public static void greet() {
    System.out.println("Hello, welcome to Java!");
}
```

Here,

* `public`: Anyone can access it.
    
* `static`: Can be used without creating an object.
    
* `void`: Doesn’t return anything.
    
* `greet()`: Function name.
    

### **How to Call a Function?**

```java
public static void main(String[] args) {
    greet();  // Calling the function
}
```

And boom! It prints:

```java
Hello, welcome to Java!
```

### **Functions with Parameters (Passing Values)**

```java
public static void sum(int a, int b) {
    System.out.println("Sum: " + (a + b));
}
```

Calling `sum(5, 10);` prints:

```java
Sum: 15
```

### **Functions that Return Values**

```java
public static int multiply(int x, int y) {
    return x * y;
}
```

Calling `multiply(3, 4);` returns `12`.

---

## **Day 3: Arrays – Storing Multiple Values Like a Boss**

Now, let’s talk about **arrays**, because apparently, storing a single value in a variable wasn’t enough.

### **What is an Array?**

An **array** is like a **container** that holds **multiple values of the same type**.

### **Declaring and Initializing an Array**

```java
int[] numbers = {10, 20, 30, 40, 50};
```

Here, `numbers` is an **array** that stores 5 integers.

### **Accessing Elements in an Array**

Each element in an array has an **index** (starting from `0`):

```java
System.out.println(numbers[0]);  // Output: 10
System.out.println(numbers[3]);  // Output: 40
```

### **Looping Through an Array**

```java
for (int i = 0; i < numbers.length; i++) {
    System.out.println(numbers[i]);
}
```

This prints all elements of the array.

### **Modifying an Array**

```java
numbers[2] = 100;  // Changes the third element (index 2) to 100
```

---

## **Day 4: Switch Statements – The If-Else Alternative**

If **if-else** statements were **annoying**, then meet **switch statements**, which make code **cleaner** and **easier to read**.

### **Basic Switch Statement**

```java
int day = 3;

switch (day) {
    case 1:
        System.out.println("Monday");
        break;
    case 2:
        System.out.println("Tuesday");
        break;
    case 3:
        System.out.println("Wednesday");
        break;
    default:
        System.out.println("Invalid Day");
}
```

Output:

```java
Wednesday
```

* The `break` statement **prevents fall-through** (i.e., stopping execution after the correct case runs).
    
* The `default` case **runs when no case matches**.
    

### **Nested Switch (Switch Inside a Switch 🤯)**

```java
int branch = 2;
int year = 3;

switch (branch) {
    case 1:
        System.out.println("CSE");
        switch (year) {
            case 1:
                System.out.println("First Year");
                break;
            case 2:
                System.out.println("Second Year");
                break;
        }
        break;
    case 2:
        System.out.println("IT");
        break;
}
```

If `branch = 1` and `year = 2`, the output will be:

```java
CSE
Second Year
```

---

## **Final Thoughts**

So, in just **4 days**, I’ve learned:  
✅ How Java works (JDK, JRE, JVM)  
✅ How to **take input and print output**  
✅ How to use **if-else and loops**  
✅ How to **write functions and reuse code**  
✅ How to **store multiple values using arrays**  
✅ How to **write cleaner code using switch statements**

Today’s **recap day** really helped me **reinforce my knowledge**, and I’m excited for what’s next! 🚀

---

That’s all for today! **Tomorrow, I’ll be back with more Java adventures.** 😎