📘 README.md
# Reverse Pyramid Pattern in Java

## 📌 Problem Statement
This program prints a simple **reverse pyramid pattern** using nested loops in Java.

### Pattern to Print:


12345
1234
123
12
1


---

## ⚙️ How It Works
1. The **outer loop** runs from 5 down to 1 (representing the number of rows).
2. The **inner loop** runs from 1 up to the current row number (`i`) to print numbers in sequence.
3. After each row, `System.out.println()` moves to the next line.

---

## ▶️ Running the Program
1. Save the code in a file named `Main.java`.
2. Compile the program:
   ```bash
   javac Main.java


Run the program:

java Main

📝 Example Output
12345
1234
123
12
1

💡 Concepts Used

Nested for loops

Java basic I/O (System.out.print and System.out.println)
```
public class Main {
    public static void main(String[] args) {
        // Outer loop controls the number of rows (from 5 down to 1)
        for (int i = 5; i >= 1; i--) {
            
            // Inner loop prints numbers from 1 up to the current row number (i)
            for (int j = 1; j <= i; j++) {
                System.out.print(j);  // Print numbers in the same row without newline
            }
            
            // Move to the next line after printing each row
            System.out.println();
        }
    }
}
```
