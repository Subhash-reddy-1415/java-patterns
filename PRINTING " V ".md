✅ Java Code for Single “V” Pattern
public class SingleVPattern {
    public static void main(String[] args) {
        int n = 7; // height of the V

        for (int i = 0; i < n; i++) {
            // Print leading spaces
            for (int j = 0; j < i; j++) {
                System.out.print(" ");
            }

            // Print left side of V
            System.out.print("*");

            // Print middle spaces between arms of V
            for (int j = 0; j < (2 * (n - i) - 3); j++) {
                System.out.print(" ");
            }

            // Print right side of V (skip last * on bottom row)
            if (i != n - 1) {
                System.out.print("*");
            }

            System.out.println();
        }
    }
}

▶️ Output for n = 7
*           *
 *         *
  *       *
   *     *
    *   *
     * *
      *


That’s a clean single V shape. 👌

📘 README.md
# Single V Pattern Printing in Java

This project prints a **single V** in a star (`*`) pattern using Java.

---

## 📌 Program Description
The program uses nested loops to print a **V-shaped** pattern:
- Stars (`*`) form two slanting arms meeting at the bottom.
- The number of spaces decreases as rows increase.

---

## 📝 Code

```java
public class SingleVPattern {
    public static void main(String[] args) {
        int n = 7; // height of the V

        for (int i = 0; i < n; i++) {
            // Print leading spaces
            for (int j = 0; j < i; j++) {
                System.out.print(" ");
            }

            // Print left side of V
            System.out.print("*");

            // Print middle spaces between arms of V
            for (int j = 0; j < (2 * (n - i) - 3); j++) {
                System.out.print(" ");
            }

            // Print right side of V (skip last * on bottom row)
            if (i != n - 1) {
                System.out.print("*");
            }

            System.out.println();
        }
    }
}

▶️ Example Output

For n = 7:

*           *
 *         *
  *       *
   *     *
    *   *
     * *
      *

🚀 How to Run

Save the file as SingleVPattern.java

Compile and run:

javac SingleVPattern.java
java SingleVPattern
