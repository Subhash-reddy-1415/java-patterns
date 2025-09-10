📘 README.md
# Right Triangle Pattern with Numbers (Java)

## 📌 Problem Statement
Write a Java program to print a right triangle pattern where each row `i` contains numbers from **1 to i**.

---

## 📝 Sample Output


1
1 2
1 2 3
1 2 3 4
1 2 3 4 5


---

## ⚙️ How It Works
1. The **outer loop** (`i`) runs from 1 to 5 → this decides the number of rows.
2. The **inner loop** (`j`) runs from 1 up to `i` → this prints numbers for each row.
3. Each number is printed with a space (`" "`).
4. After each row, a newline is printed to move to the next row.

---

## ▶️ Running the Program
1. Save the file as `Main.java`.
2. Compile the program:
   ```bash
   javac Main.java


Run the program:

java Main

💡 Concepts Used

Nested for loops

Pattern printing

Java console output (System.out.print and System.out.println)
```
public class Main {
    public static void main(String[] args) {
        // Outer loop controls the number of rows (from 1 to 5)
        for (int i = 1; i <= 5; i++) {
            
            // Inner loop prints numbers from 1 up to the current row number (i)
            for (int j = 1; j <= i; j++) {
                System.out.print(j + " ");  // Print numbers in the same row with a space
            }
            
            // Move to the next line after each row
            System.out.println();
        }
    }
}
```
