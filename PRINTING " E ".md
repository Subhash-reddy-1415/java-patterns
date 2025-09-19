📄 README.md
# Java Alphabet Pattern – Letter E

This project demonstrates how to print the English alphabet **E** using star (`*`) patterns in Java.  
It uses **nested loops** (`for`) and **conditional statements** (`if-else`) to generate the shape.

---

## 📌 Program Explanation
- The program prints a **12 × 12 grid**.
- Stars (`*`) are printed when:
  - `i == 0` → Top border  
  - `i == 6` → Middle bar  
  - `i == 11` → Bottom border  
  - `j == 0` → Left border  
- Spaces are printed elsewhere to form the shape of the letter **E**.

---

## 🖥️ Code
```java
public class E {
    public static void main(String[] args) {
        for (int i = 0; i <= 11; i++) {
            for (int j = 0; j <= 11; j++) {
                if (i == 0 || i == 11 || i == 6 || j == 0) {
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
* * * * * * * * * * * * 

🚀 How to Run

Save the file as E.java

Compile the program:

javac E.java


Run the program:

java E
