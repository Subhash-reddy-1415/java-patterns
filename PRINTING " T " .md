📘 README.md
# T Pattern Printing in Java

This project prints the alphabet **T** in a star (`*`) pattern using Java.

---

## 📌 Program Description
The program uses nested loops to print the **T** character:
- Top horizontal line (`*******`)
- Center vertical line

---

## 📝 Code

```java
public class TPattern {
    public static void main(String[] args) {
        int n = 7;  // height of the pattern

        for (int i = 0; i < n; i++) {
            // Top horizontal line
            if (i == 0) {
                for (int j = 0; j < n; j++) {
                    System.out.print("*");
                }
            } 
            // Vertical line
            else {
                for (int j = 0; j < n; j++) {
                    if (j == n / 2) {
                        System.out.print("*");
                    } else {
                        System.out.print(" ");
                    }
                }
            }
            System.out.println();
        }
    }
}

▶️ Example Output

For n = 7, the output will be:

*******
   *   
   *   
   *   
   *   
   *   
   *   

🚀 How to Run

Save the file as TPattern.java

Open terminal and compile:

javac TPattern.java


Run the program:

java TPattern
