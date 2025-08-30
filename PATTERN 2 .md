⭐ Java Pattern Program – Rectangle of Stars

This repository demonstrates a basic Java pattern printing program. The task is to print a rectangle of stars using nested for loops. This exercise helps beginners strengthen their understanding of loop structures in Java.

📌 Problem Statement

Develop a simple Java application to print the following star pattern:

*****
*****
*****
*****

Task Instructions:

Use an outer loop to represent the number of rows (4 rows).

Use an inner loop to represent the number of columns (5 stars in each row).

Inside the inner loop, print "*" without moving to the next line.

After completing the inner loop, use System.out.println() to move to the next row.

💡 Key Concepts Learned

✅ Nested for loops in Java

✅ Difference between System.out.print() and System.out.println()

✅ Basic console output formatting

✅ Problem-solving using step-by-step iteration

Code
,,,
public class Pattern {
    public static void main(String[] args) {
        // Outer loop controls number of rows
        for (int row = 1; row <= 4; row++) {
            
            // Inner loop controls number of stars per row
            for (int col = 1; col <= 5; col++) {
                System.out.print("*"); // Print star without newline
            }
            
            // Move to the next line after each row
            System.out.println();
        }
    }
}
```

🛠️ How to Run

Follow these steps to run the program:

Save the file as Pattern.java

Open a terminal/command prompt in the folder where the file is saved

Compile the program:

javac Pattern.java


Run the compiled program:

java Pattern

📖 Expected Output

When you run the program, the following output will be displayed:

*****
*****
*****
*****
