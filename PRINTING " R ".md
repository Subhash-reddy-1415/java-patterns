# R Pattern Printing in Java

This project prints the alphabet **R** in a star (`*`) pattern using Java.

---

## 📌 Program Description
The program uses nested loops to print the **R** character:
- Left vertical line
- Top horizontal line
- Middle horizontal line
- Upper right vertical line
- Diagonal leg forming the slant of "R"

---

## 📝 Code

```java
public class RPattern {
    public static void main(String[] args) {
        int n = 7;  // height of the pattern

        for (int i = 0; i < n; i++) {
            System.out.print("*"); // left vertical line

            // for top and middle horizontal line
            if ((i == 0) || (i == n / 2)) {
                for (int j = 0; j < n - 2; j++) {
                    System.out.print("*");
                }
            } 
            // for upper right vertical line
            else if (i < n / 2) {
                for (int j = 0; j < n - 2; j++) {
                    if (j == n - 3) {
                        System.out.print("*");
                    } else {
                        System.out.print(" ");
                    }
                }
            }
            // for diagonal leg of R
            else {
                for (int j = 0; j <= i - (n / 2); j++) {
                    System.out.print(" ");
                }
                System.out.print("*");
            }

            System.out.println();
        }
    }
}
▶️ Example Output
For n = 7, the output will be:

markdown
Copy code
*****
*   *
*   *
*****
*  *
*   *
*    *
🚀 How to Run
Save the file as RPattern.java

Open terminal and compile:

bash
Copy code
javac RPattern.java
Run the program:

bash
Copy code
java RPattern
