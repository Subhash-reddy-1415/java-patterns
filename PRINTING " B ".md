📘 README.md
# Java Pattern Printing - Letter "B"

This program prints a block-style letter **B** using nested loops in Java.

## 📂 File Structure
- `B.java` → Java source file containing the code.

## 🖥️ Output
When run, the program prints:


                * 

                * 

                * 

                * 

                * 

                * 

                * 

                * 


This visually resembles the capital letter **B**.

## ⚙️ How It Works
1. Two nested `for` loops:
   - Outer loop (`i`) → rows (`1 to 11`).
   - Inner loop (`j`) → columns (`0 to 11`).
2. Prints `*` when:
   - Row is first (`i == 1`) → top border
   - Row is last (`i == 11`) → bottom border
   - Column is first (`j == 0`) → left border
   - Column is last (`j == 11`) → right border
   - Row is middle (`i == 11 / 2`) → center line
3. Otherwise, prints spaces to keep the shape.

## ▶️ How to Run
1. Compile the Java file:
   ```bash
   javac B.java


Run the program:

java B
```
public class B {

    public static void main(String[] args) {
        // Outer loop → controls rows (1 to 11)
        for (int i = 1; i <= 11; i++) {
            
            // Inner loop → controls columns (0 to 11)
            for (int j = 0; j <= 11; j++) {
                
                // Print '*' in the following cases:
                // 1. Top border (i == 1) → first row
                // 2. Bottom border (i == 11) → last row
                // 3. Left border (j == 0) → first column
                // 4. Right border (j == 11) → last column
                // 5. Middle horizontal line (i == 11 / 2) → row 5 (since 11/2 = 5 in integer division)
                if (i == 1 || i == 11 || j == 0 || j == 11 || i == 11 / 2) {
                    System.out.print("* ");
                } else {
                    // Print space for empty positions
                    System.out.print("  ");
                }
            }
            
            // Move to the next row
            System.out.println();
        }
    }
}
```
