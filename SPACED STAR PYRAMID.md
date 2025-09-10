📘 README.md
# Right-Aligned Triangle Pattern with Asterisks (Java)

## 📌 Problem Statement
Write a Java program to print a **right-aligned triangle** pattern using `*`.

---

## 📝 Sample Output

*


*


---

## ⚙️ How It Works
1. The **outer loop** (`i`) runs from 1 to 5 → represents the number of rows.
2. The **first inner loop** (`j`) prints spaces → ensures the stars align to the right.
3. The **second inner loop** (`k`) prints stars (`*`) followed by a space.
4. After printing each row, `System.out.println()` moves to the next line.

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

Space management in pattern printing

Right-alignment with spaces
```
public class Main {
    public static void main(String[] args) {
        // Outer loop controls the number of rows (1 to 5)
        for (int i = 1; i <= 5; i++) {
            
            // First inner loop prints spaces (decreasing as row increases)
            for (int j = 5; j > i; j--) {
                System.out.print(" ");  // Print space for right alignment
            }
            
            // Second inner loop prints asterisks (*) with a space
            for (int k = 1; k <= i; k++) {
                System.out.print("* ");  // Print star followed by a space
            }
            
            // Move to the next line after each row
            System.out.println();
        }
    }
}
```
