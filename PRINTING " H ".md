⭐ Java Program to Print Letter H
📌 Description

This program prints the alphabet H using asterisks (*).
It uses nested loops and conditional statements to determine star (*) and space ( ) positions.

📂 File

H.java

⚙️ How It Works

Outer loop → Controls rows (i)

Inner loop → Controls columns (j)

Condition:

Print * if:

First column (j == 0)

Last column (j == n)

Middle row (i == n/2)

Otherwise, print spaces.

▶️ How to Run

Install Java JDK
.

Save the file as H.java.

Open terminal and navigate to the folder.

Compile:

javac H.java


Run:

java H

📌 Sample Output

For n = 10:

*                   * 
*                   * 
*                   * 
*                   * 
*                   * 
* * * * * * * * * * * 
*                   * 
*                   * 
*                   * 
*                   * 
*                   * 

📘 Learning Goals

Practice nested loops in Java

Learn how to print alphabet patterns with conditions

Understand row and column logic for shapes
```
public class H {
    public static void main(String[] args) {
        int n = 11; // height of the letter

        for (int i = 0; i <= n; i++) {
            for (int j = 0; j <= n; j++) {
                // Left vertical line, right vertical line, or middle horizontal bar
                if (j == 0 || j == n || i == n / 2) {
                    System.out.print("* ");
                } else {
                    System.out.print("  ");
                }
            }
            System.out.println();
        }
    }
}
```
