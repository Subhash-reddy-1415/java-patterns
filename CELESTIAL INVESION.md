📘 README.md
# Inverted Pyramid Pattern with Asterisks (Java)

## 📌 Problem Statement
Write a Java program to print an **inverted pyramid pattern** using `*`.

---

## 📝 Sample Output


**
*


---

## ⚙️ How It Works
1. The **outer loop** (`i`) starts from 5 and decreases to 1 → represents the number of rows.
2. The **inner loop** (`j`) runs from 1 up to `i` → prints `*` for each column in that row.
3. After each row, a newline is added using `System.out.println()`.

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

Pattern printing with characters

Java console output (System.out.print, System.out.println)
```
public class Main {
    public static void main(String[] args) {
        // Outer loop controls the number of rows (from 5 down to 1)
        for (int i = 5; i >= 1; i--) {
            
            // Inner loop prints '*' up to the current row number (i)
            for (int j = 1; j <= i; j++) {
                System.out.print("*");  // Print star without newline
            }
            
            // Move to the next line after printing each row
            System.out.println();
        }
    }
}
```
