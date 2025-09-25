Letter N Pattern in Java
📌 Overview

This Java program prints the letter N using a pattern of asterisks (*).
The program uses nested loops and conditional checks to draw the two vertical bars and the diagonal of the letter N.

📝 Features

Prints the letter N with a customizable height.

Uses simple nested for loops.

Demonstrates pattern printing logic in Java.

💻 Code
public class N {
    public static void main(String[] args) {
        int n = 10; // size of the letter (height)

        for (int i = 0; i <= n; i++) { // rows
            for (int j = 0; j <= n; j++) { // columns
                if (j == 0 || j == n || i == j) { 
                    // left bar || right bar || diagonal
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
*                   * 
* *                 * 
*   *               * 
*     *             * 
*       *           * 
*         *         * 
*           *       * 
*             *     * 
*               *   * 
*                 * * 
*                   * 

🚀 How to Run

Save the program as N.java

Open terminal/command prompt and compile:

javac N.java


Run the program:

java N
