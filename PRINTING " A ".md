📘 README.md
# Java Pattern Printing - Letter "A"

This project prints a pattern in the shape of the letter **A** using nested loops in Java.

## 📂 File Structure
- `A.java` → The main Java source file that contains the code.

## 🖥️ Output
When you run the program, it prints:


              * 

              * 

              * 

              * 

              * 

              * 

              * 

              * 

              * 


This output visually represents the capital letter **A**.

## ⚙️ How It Works
1. Uses two nested `for` loops:
   - Outer loop (`i`) → controls rows (1 to 11).
   - Inner loop (`j`) → controls columns (1 to 11).
2. Prints `*` at specific positions:
   - Top border (`i == 1`)
   - Middle horizontal line (`i == 5`)
   - Left border (`j == 1`)
   - Right border (`j == 11`)
3. Prints spaces `"  "` elsewhere to maintain alignment.

## ▶️ How to Run
1. Compile the Java file:
   ```bash
   javac A.java


Run the program:

java A


You should see the A pattern printed on the console.
```
public class A {

    public static void main(String[] args) {
        // Outer loop → controls the number of rows (i ranges from 1 to 11)
        for (int i = 1; i <= 11; i++) {
            
            // Inner loop → controls the number of columns (j ranges from 1 to 11)
            for (int j = 1; j <= 11; j++) {
                
                // Print '*' in the following cases:
                // 1. First row (i == 1)
                // 2. Fifth row (i == 5)
                // 3. First column (j == 1)
                // 4. Last column (j == 11)
                if (i == 1 || i == 5 || j == 1 || j == 11) {
                    System.out.print("* ");
                } else {
                    // Otherwise, print spaces
                    System.out.print("  ");
                }
            }
            
            // Move to the next line after each row
            System.out.println();
        }
    }
}
```
