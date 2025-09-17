📘 README
Pattern Printing Program

Filename: Main.java
Language: Java

📋 Description

This Java program prints a hollow square pattern using nested for loops.

Pattern Output:

*****
*   *
*   *
*   *
*****

⚙️ How It Works

The pattern is 5x5 (can be changed using variable n).

Outer loop (i) runs for each row from 1 to n.

Inner loop (j) runs for each column from 1 to n.

* is printed when:

It is the first or last row (i == 1 || i == n)

OR the first or last column (j == 1 || j == n)

Otherwise, a space is printed.

▶️ How to Run

Save the code in a file named Main.java.

Open a terminal/command prompt.

Compile the code:

javac Main.java


Run the program:

java Main

✏️ Customization

Change n value to adjust pattern size.
Example: int n = 7; will produce a 7x7 hollow square.
```
public class Main {
    public static void main(String[] args) {
        int n = 5; // Size of the pattern

        for (int i = 1; i <= n; i++) {          // Outer loop for rows
            for (int j = 1; j <= n; j++) {      // Inner loop for columns
                // Print '*' on first or last row OR first or last column
                if (i == 1 || i == n || j == 1 || j == n) {
                    System.out.print("*");
                } else {
                    System.out.print(" ");
                }
            }
            System.out.println(); // Move to next line after each row
        }
    }
}
```
