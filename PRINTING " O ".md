Letter O Pattern in Java
📌 Overview

This Java program prints the letter O using asterisks (*).
It uses nested loops to form the outer boundary of the letter, leaving the inside hollow.

📝 Features

Prints the letter O with a customizable size.

Uses simple nested for loops and conditions.

Demonstrates pattern printing logic in Java.

💻 Code
public class O {
    public static void main(String[] args) {
        int n = 10; // size of the letter (height & width)

        for (int i = 0; i <= n; i++) {  // rows
            for (int j = 0; j <= n; j++) { // columns
                if (i == 0 || i == n || j == 0 || j == n) {
                    // top row || bottom row || left bar || right bar
                    System.out.print("* ");
                } else {
                    System.out.print("  ");
                }
            }
            System.out.println();
        }
    }
}

▶️ Example Output (for n = 10)
* * * * * * * * * * * 
*                   * 
*                   * 
*                   * 
*                   * 
*                   * 
*                   * 
*                   * 
*                   * 
*                   * 
* * * * * * * * * * * 

🚀 How to Run

Save the file as O.java

Open terminal/command prompt and compile:

javac O.java


Run the program:

java O
