README – Print Pattern 11 (Java)
📌 Problem Statement

You need to develop a simple Java application to print a diamond-shaped star pattern using nested loop structures.

Pattern to Print:
    *
   * *
  * * *
 * * * *
* * * * *
 * * * *
  * * *
   * *
    *

🛠️ Approach

This pattern can be divided into two halves:

Upper Half (Pyramid Shape)

Print spaces before stars.

Print stars followed by a space ("* ").

Lower Half (Inverted Pyramid Shape)

Similar logic, but the row count decreases.

Key Points:

Use an outer loop for rows.

Use one inner loop for spaces.

Use another inner loop for stars.

Print stars with spaces ("* ") for alignment.

Use System.out.println() at the end of each row.

💻 Java Code
```
public class Main {
    public static void main(String[] args) {
        // Upper half of the diamond
        for (int i = 1; i <= 5; i++) {
            // Print spaces
            for (int j = 5; j > i; j--) {
                System.out.print(" ");
            }
            // Print stars
            for (int k = 1; k <= i; k++) {
                System.out.print("* ");
            }
            // Move to next line
            System.out.println();
        }

        // Lower half of the diamond
        for (int i = 4; i >= 1; i--) {
            // Print spaces
            for (int j = 5; j > i; j--) {
                System.out.print(" ");
            }
            // Print stars
            for (int k = 1; k <= i; k++) {
                System.out.print("* ");
            }
            // Move to next line
            System.out.println();
        }
    }
}
```

📊 Dry Run (Upper Half Example)

For i = 3 (3rd row):

Spaces → 2 spaces (5 - 3)

Stars → 3 stars with space (* * * )

Printed line → " * * * "

✅ Final Output
    *
   * *
  * * *
 * * * *
* * * * *
 * * * *
  * * *
   * *
    *

📌 Key Concepts Used

Nested loops (outer controls rows, inner controls spaces & stars).

Pattern symmetry (first increasing stars, then decreasing).

String alignment using spaces.

🚀 How to Run

Save the code as Main.java.

Compile:

javac Main.java


Run:

java Main
