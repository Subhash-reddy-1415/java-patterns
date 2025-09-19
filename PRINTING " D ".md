🖥️ Java Code for Letter D
public class D {
    public static void main(String[] args) {
        for (int i = 0; i <= 11; i++) {          // rows
            for (int j = 0; j <= 11; j++) {      // columns
                if (i == 0 || i == 11 || j == 0 || j == 11) {
                    System.out.print("* ");
                } else {
                    System.out.print("  ");
                }
            }
            System.out.println();
        }
    }
}

📄 README.md
# Java Alphabet Pattern – Letter D

This project demonstrates how to print the English alphabet **D** using star (`*`) patterns in Java.  
It uses **nested loops** (`for`) and **conditional statements** (`if-else`) to generate the shape.

---

## 📌 Program Explanation
- The program prints a **12 × 12 grid**.
- Stars (`*`) are printed when:
  - `i == 0` → Top border  
  - `i == 11` → Bottom border  
  - `j == 0` → Left border  
  - `j == 11` → Right border  
- Spaces are printed elsewhere to form the shape of the letter **D**.

---

## 🖥️ Code
```java
public class D {
    public static void main(String[] args) {
        for (int i = 0; i <= 11; i++) {
            for (int j = 0; j <= 11; j++) {
                if (i == 0 || i == 11 || j == 0 || j == 11) {
                    System.out.print("* ");
                } else {
                    System.out.print("  ");
                }
            }
            System.out.println();
        }
    }
}

🎯 Sample Output
* * * * * * * * * * * * 
*                     *
*                     *
*                     *
*                     *
*                     *
*                     *
*                     *
*                     *
*                     *
*                     *
* * * * * * * * * * * * 

🚀 How to Run

Save the file as D.java

Compile the program:

javac D.java


Run the program:

java D
