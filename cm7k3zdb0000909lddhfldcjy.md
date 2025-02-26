---
title: "Day 1: Java Basics – Why Am I Doing This to Myself?"
seoTitle: "Java Basics: Understanding the Essentials"
seoDescription: "Starting Java with "Hello, World!" and exploring basics like JDK, JVM, memory management, and simple I/O. A journey into Java's intriguing world"
datePublished: Tue Feb 25 2025 06:31:39 GMT+0000 (Coordinated Universal Time)
cuid: cm7k3zdb0000909lddhfldcjy
slug: day-1-java-basics-why-am-i-doing-this-to-myself
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1740464984894/f461bb03-c7db-464b-abc4-e4800f72843a.webp
tags: java, data-structures, wemakedevs

---

So, I started learning **Java** today because apparently, printing `"Hello, World!"` is the first step toward greatness. I followed **Kunal Kushwaha’s** resources, and well… Java is already throwing new words at me. Here’s what I learned (and somehow survived).

---

## **Programming Languages -** Because One Doesn't Fit All

Turns out, there are different types of programming languages. Because why keep things simple?

1. **Compiled Languages** – These translate the whole code at once before running it. (Like turning in your homework and praying there are no mistakes.) Examples: **C, C++**.
    
2. **Interpreted Languages** – These read and run the code **line by line** (kind of like someone reading a book out loud). Examples: **Python, JavaScript**.
    
3. **Java (Hybrid)** – Java **compiles** first, then **runs inside a Virtual Machine (JVM)**. Basically, Java doesn’t trust me to run code directly, so it checks everything first.
    

---

## **Java Environments –** Because Java Needs an Entire Toolbox

### **1\. JDK (Java Development Kit)**

This is **everything I need to write and run Java programs**. It includes:

* **JRE (Java Runtime Environment)** – So I can run Java programs.
    
* **Java Compiler** – Translates my code into something Java understands.
    
* **Other Developer Tools** – To help me debug, compile, and probably cry less.
    

### **2\. JRE (Java Runtime Environment)**

This is **only needed to run Java programs**, not write them. If all I want is to run Java apps (not code them), JRE is enough.

### **3\. JVM (Java Virtual Machine)**

The **JVM** is the real magician here. It runs Java code **on any operating system** by converting it into something my computer understands. That’s why Java is "Write Once, Run Anywhere" (or in my case, "Write Once, Debug Everywhere").

---

## **Memory Management – Where My Variables Live**

Java actually cares about where it stores stuff. Here’s how it works:

* **Stack Memory** – Quick, temporary storage for small stuff (like method calls and variables).
    
* **Heap Memory** – Stores objects and is managed by **Garbage Collector** (so I don’t have to clean up my own mess—nice).
    

In short, Java is smart enough to manage memory, but if I mess up, it will still remind me with an error message.

---

## **Installing Java – Step 1 of the Struggle**

Before I can even write code, I had to install **JDK (Java Development Kit)** from [oracle.com](https://www.oracle.com/java/) or use OpenJDK.

To check if it worked, I ran this command:

```sh
java -version
```

If Java responded, great! If not, well… time to Google the problem (which I’m sure will happen a lot).

---

## **Writing My First Java Program – The Famous "Hello, World!"**

Here’s the **first-ever** Java program everyone writes:

```java
public class Main {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```

### **Breaking It Down (Because Java Loves Fancy Words)**

* `public class Main` – Creates a class (basically a container for my code).
    
* `public static void main(String[] args)` – This is the main method. Java won’t run without it.
    
* `System.out.println("Hello, World!");` – Prints text to the screen (so I can pretend I did something important).
    

Ran it. It worked. I felt smart for five seconds.

---

## **Taking Input & Output – Letting Users Type Stuff**

Java is not a mind reader, so if I want input, I have to **ask** for it. Here’s how:

```java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter your name: ");
        String name = sc.nextLine();
        System.out.println("Hello, " + name + "!");
    }
}
```

### **What’s Happening Here?**

* `import java.util.Scanner;` – Brings in the Scanner (so Java knows how to take input).
    
* `Scanner sc = new Scanner(System.in);` – Creates a Scanner object (basically a keyboard listener).
    
* `sc.nextLine();` – Reads what the user types.
    

Tried it. It worked. Now Java can actually interact with me instead of just printing stuff.

---

## **Conditionals & Loops – Making Java Think**

### **If-Else (Making Decisions)**

I can tell Java to **do different things based on conditions**:

```java
int age = 18;

if (age >= 18) {
    System.out.println("You can vote!");
} else {
    System.out.println("Too young, sorry.");
}
```

Java is now judging people based on their age. Cool.

---

### **Loops (Making Java Repeat Stuff)**

#### **For Loop (Runs a Fixed Number of Times)**

```java
for (int i = 1; i <= 5; i++) {
    System.out.println("This is loop number " + i);
}
```

Java will run this **five times**. Good for repetitive tasks (or annoying people).

#### **While Loop (Runs Until I Say Stop)**

```java
int x = 1;
while (x <= 5) {
    System.out.println("Still looping...");
    x++;
}
```

This loop runs **as long as the condition is true**. If I forget to update `x`, it **never stops** (which is how I accidentally crashed my code).

---

## **What I Learned Today**

* Java **compiles and interprets** code because it likes to be special.
    
* There are **JDK, JRE, and JVM**, and yes, I need to remember what they do.
    
* Memory is managed by **Java’s Garbage Collector**, so I don’t have to worry (until I do).
    
* I can finally **print stuff, take input, and use loops** without breaking everything (well, most of the time).
    

### **What’s Next?**

Tomorrow, I’ll dive deeper into **functions, arrays, and maybe recursion (if I’m brave enough).** Stay tuned!

---