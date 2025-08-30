Print Pattern 1 in Java
📌 Problem Statement

You need to develop a simple Java application to print a given pattern using a loop structure.

Pattern to Print:
*
*
*
*

📝 Explanation

We need to print the * symbol 4 times, each on a new line.

This can be done using a for loop that iterates 4 times.

Inside the loop, System.out.println("*"); is used to print the asterisk on a new line each time.

💻 Code
```
public class Main {
    public static void main(String[] args) {
        // Loop runs 4 times
        for (int i = 1; i <= 4; i++) {
            // Print star on a new line
            System.out.println("*");
        }
    }
}
```

▶️ Output
*
*
*
*

📖 Concepts Used

For Loop → To repeat printing 4 times.

System.out.println() → Prints output with a new line after each star.

✅ This is the first basic pattern printing program in Java.
