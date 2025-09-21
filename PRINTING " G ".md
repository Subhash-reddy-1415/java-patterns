📄 README.md
# Java Alphabet Pattern – Letter G

This project demonstrates how to print the English alphabet **G** using star (`*`) patterns in Java.  
It uses **nested loops** and **conditions** to mimic the structure of the letter.

---

## 📌 Program Explanation
- The program draws a **12×12 grid** of stars and spaces.
- Stars are printed at positions:
  - `i == 0` → Top horizontal bar  
  - `i == n` → Bottom horizontal bar  
  - `j == 0` → Left vertical bar  
  - `j == n && i >= n/2` → Right vertical bar (only lower half)  
  - `i == n/2 && j >= n/2` → Small middle horizontal bar inside G  

---

## 🖥️ Code
```java
public class G {
    public static void main(String[] args) {
        int n = 11;
        for (int i = 0; i <= n; i++) {
            for (int j = 0; j <= n; j++) {
                if (i == 0 || i == n || j == 0 || (j == n && i >= n/2) || (i == n/2 && j >= n/2)) {
                    System.out.print("* ");
                } else {
                    System.out.print("  ");
                }
            }
            System.out.println();
        }
    }
}

🎯 Sample Output (n = 11)
* * * * * * * * * * * * 
*                       
*                       
*                       
*                       
*         * * * * * * * 
*                     * 
*                     * 
*                     * 
*                     * 
*                     * 
* * * * * * * * * * * * 

🚀 How to Run

Save the file as G.java

Compile:

javac G.java


Run:

java G
 
