📘 README.md
# W Pattern Printing in Java

This project prints the alphabet **W** in a star (`*`) pattern using Java.

---

## 📌 Program Description
The program uses nested loops to print the **W** character:
- It consists of **four legs** (two on each side) forming the “W” shape.
- The middle two legs cross diagonally near the bottom.

---

## 📝 Code

```java
public class WPattern {
    public static void main(String[] args) {
        int n = 7; // height of the W

        for (int i = 0; i < n; i++) {
            // First vertical line
            System.out.print("*");

            // Space between 1st and 2nd leg
            for (int j = 0; j < n - 1; j++) {
                if (j == i) {
                    System.out.print("*");
                } else {
                    System.out.print(" ");
                }
            }

            // Space between 2nd and 3rd leg
            for (int j = n - 2; j >= 0; j--) {
                if (j == i) {
                    System.out.print("*");
                } else {
                    System.out.print(" ");
                }
            }

            // Last vertical line
            System.out.print("*");

            System.out.println();
        }
    }
}

▶️ Example Output

For n = 7:

*     *     *
*     *     *
*     *     *
*     *     *
*     *     *
 *   * *   * 
  * *   * *  

🚀 How to Run

Save the file as WPattern.java

Open terminal and compile:

javac WPattern.java


Run the program:

java WPattern
