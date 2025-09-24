📘 Java Pattern Program – Print Letter "M"
📌 Overview

This Java program prints the letter M in a star (*) pattern using nested loops.
It demonstrates the use of conditional statements inside loops to draw vertical and diagonal lines.

🖼️ Example Output

For size n = 10:

*                   * 
* *               * * 
*   *           *   * 
*     *       *     * 
*       *   *       * 
*         *         * 
*                   * 
*                   * 
*                   * 
*                   * 
*                   * 

📝 Code
public class M {
    public static void main(String[] args) {
        int n = 10; // size of the letter (height)

        for (int i = 0; i <= n; i++) {  // rows
            for (int j = 0; j <= n; j++) { // columns

                // Conditions for M
                if (j == 0 || j == n ||          // left and right vertical bars
                    (i == j && i <= n/2) ||      // left diagonal (top half)
                    (i + j == n && i <= n/2)) {  // right diagonal (top half)
                    System.out.print("* ");
                } else {
                    System.out.print("  ");
                }
            }
            System.out.println();
        }
    }
}

⚙️ How It Works

Outer Loop (i) → Controls the number of rows (height).

Inner Loop (j) → Controls the number of columns (width).

Conditions:

j == 0 → Prints the left vertical line.

j == n → Prints the right vertical line.

i == j && i <= n/2 → Prints the left diagonal in the top half.

i + j == n && i <= n/2 → Prints the right diagonal in the top half.

🚀 Usage

Copy the code into a file named M.java

Compile the program:

javac M.java


Run the program:

java M

🎯 Learning Outcome

Understand nested loops in Java.

Learn to apply conditions to create patterns.

Practice constructing letters with ASCII-art style programming.
