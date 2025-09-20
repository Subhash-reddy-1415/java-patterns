# Java Alphabet Pattern – Letter F

This project demonstrates how to print the English alphabet **F** using star (`*`) patterns in Java.  
It uses **nested loops** (`for`) and **conditional statements** (`if-else`) to generate the shape.

---

## 📌 Program Explanation
- The program prints a **12 × 12 grid**.
- Stars (`*`) are printed when:
  - `i == 0` → Top horizontal bar  
  - `i == 6` → Middle horizontal bar  
  - `j == 0` → Left vertical bar  
- Spaces are printed elsewhere to form the shape of the letter **F**.

---

## 🖥️ Code
```java
public class F {
    public static void main(String[] args) {
        for (int i = 0; i <= 11; i++) {
            for (int j = 0; j <= 11; j++) {
                if (i == 0 || i == 6 || j == 0) {
                    System.out.print("* ");
                } else {
                    System.out.print("  ");
                }
            }
            System.out.println();
        }
    }
}
```
* * * * * * * * * * * * 
* 
* 
* 
* 
* 
* * * * * * * * * * * * 
* 
* 
* 
* 
* 

🚀 How to Run

Save the file as F.java

Compile the program:

javac F.java


Run the program:

java F
