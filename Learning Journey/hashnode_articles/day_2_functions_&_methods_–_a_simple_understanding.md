# Day 2: Functions & Methods – A Simple Understanding

So today, I learned about **functions and methods in Java**. Basically, instead of writing the same code **again and again** like a **copy-paste champion**, I can just write a function **once** and call it whenever needed.

It’s like **ordering pizza**—instead of making one from scratch every time, you just **call the pizza shop**, and they handle it. Functions work the same way! **Write once, use forever** (or at least until Java decides to throw an error).

---

## **What is a Function?** 🤔

A **function** is a block of code that does something **specific**. Instead of writing the same logic multiple times, you just write it once inside a function and **call it** whenever needed.

Think of it like this:

* **Without functions**: You’re making tea **from scratch every time**—boiling water, adding tea leaves, sugar, milk... exhausting!
    
* **With functions**: You create a "tea-making machine" (a function). Just press a button (call the function), and it makes tea for you!
    

---

## **How Do We Write a Function?**

Java, being Java, has some rules. Here’s the basic structure of a function:

```java
returnType functionName(parameters) {
    // function body (this is where the logic goes)
    return something; 
}
```

Looks a bit scary? Don't worry, let’s break it down.

### **Example 1: A Simple Function That Adds Two Numbers**

```java
public class Main {
    // Function definition
    public static int addNumbers(int a, int b) { 
        int sum = a + b; // Adds the numbers
        return sum; // Returns the result
    }

    public static void main(String[] args) {
        int result = addNumbers(5, 10); // Calling the function
        System.out.println("Sum: " + result); // Printing the result
    }
}
```

---

## **Understanding the Function** 👀

### **Step 1: Function Definition**

```java
public static int addNumbers(int a, int b) { 
```

* `public static` → Just some Java keywords. Ignore them for now.
    
* `int` → The return type. It means this function will return an integer.
    
* `addNumbers` → The function name (you can name it whatever makes sense).
    
* `(int a, int b)` → These are **parameters** (input values for the function).
    

### **Step 2: Function Logic**

```java
int sum = a + b;
```

* Takes `a` and `b`, adds them, and stores the result in `sum`.
    

### **Step 3: Returning the Result**

```java
return sum;
```

* The function **sends back** the result to wherever it was called.
    

### **Step 4: Calling the Function**

```java
int result = addNumbers(5, 10);
```

* We **call** the function `addNumbers(5, 10)`, giving it two numbers.
    
* The function does its magic and returns `15`, which gets stored in `result`.
    

**Output:**

```bash
Sum: 15
```

---

## **Functions with No Return Type (void)**

Sometimes, we just want a function to **do something** without returning a value.

### **Example 2: A Function That Prints a Message**

```java
public class Main {
    public static void greetUser() { 
        System.out.println("Hello! Welcome to Java!");
    }

    public static void main(String[] args) {
        greetUser(); // Calling the function
    }
}
```

### **Explanation:**

* **No** `return` statement because `void` means "returns nothing."
    
* The function **just prints a message** when called.
    
* Calling `greetUser();` in `main()` runs the function.
    

**Output:**

```bash
Hello! Welcome to Java!
```

---

## **Problem: Reverse a Number Using Functions**

Now, let’s use a function to **reverse a number** (because why do it manually?).

### **Example 3: Function to Reverse a Number**

```java
public class Main {
    public static int reverseNumber(int n) {
        int rev = 0;
        while (n > 0) {
            int lastDigit = n % 10; // Extract last digit
            rev = rev * 10 + lastDigit; // Add it to the reversed number
            n = n / 10; // Remove last digit from n
        }
        return rev;
    }

    public static void main(String[] args) {
        int reversed = reverseNumber(12345);
        System.out.println("Reversed Number: " + reversed);
    }
}
```

### **How This Works:**

Let’s take `12345` and go step by step:

| Step | `n` (Original) | `lastDigit = n % 10` | `rev = rev * 10 + lastDigit` | `n = n / 10` |
| --- | --- | --- | --- | --- |
| 1 | 12345 | 5 | 0 \* 10 + 5 = **5** | 1234 |
| 2 | 1234 | 4 | 5 \* 10 + 4 = **54** | 123 |
| 3 | 123 | 3 | 54 \* 10 + 3 = **543** | 12 |
| 4 | 12 | 2 | 543 \* 10 + 2 = **5432** | 1 |
| 5 | 1 | 1 | 5432 \* 10 + 1 = **54321** | 0 (Done!) |

**Output:**

```bash
Reversed Number: 54321
```

---

## **What I Learned Today**

✔ **Functions let me reuse code** instead of writing the same thing repeatedly.  
✔ **Methods** are basically functions inside a class (and everything in Java is inside a class).  
✔ Java **forces me to return something** if the function is not `void`.  
✔ Functions make **problem-solving easier**—just break problems into small steps.

---

### **What’s Next?**

Tomorrow, I’ll tackle **arrays** (because one variable is never enough). Wish me luck—Java still has more surprises for me. 😆

---