📘 README.md
# U Pattern Printing in Java

This project prints the alphabet **U** in a star (`*`) pattern using Java.

---

## 📌 Program Description
The program uses nested loops to print the **U** character:
- Left vertical line
- Right vertical line
- Bottom horizontal line

---

## 📝 Code

```java
public class UPattern {
    public static void main(String[] args) {
        int n = 7;  // height of the pattern

        for (int i = 0; i < n; i++) {
            // Left vertical line
            System.out.print("*");

            // Spaces between left and right vertical lines
            for (int j = 0; j < n - 2; j++) {
                if (i == n - 1) {
                    // Bottom line
                    System.out.print("*");
                } else {
                    System.out.print(" ");
                }
            }

            // Right vertical line
            System.out.print("*");

            System.out.println();
        }
    }
}

▶️ Example Output

For n = 7, the output will be:

*     *
*     *
*     *
*     *
*     *
*     *
*******

🚀 How to Run

Save the file as UPattern.java

Open terminal and compile:

javac UPattern.java


Run the program:

java UPattern
