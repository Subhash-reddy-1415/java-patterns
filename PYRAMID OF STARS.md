📌 Problem Statement

Write a Java program to print the following pattern using nested loops:

*
**
***
****
*****

📝 Explanation

Use two nested loops:

Outer loop (i) → controls the number of rows (1 to 5).

Inner loop (j) → prints stars (*) in each row.

For each row i, print i stars.

After finishing each row, print a new line.

💻 Code
```
public class Main {
    public static void main(String[] args) {
        // Outer loop for rows
        for (int i = 1; i <= 5; i++) {
            
            // Inner loop for printing stars
            for (int j = 1; j <= i; j++) {
                System.out.print("*");
            }
            
            // Move to next line after each row
            System.out.println();
        }
    }
}
```

🔎 Dry Run

i = 1 → prints *

i = 2 → prints **

i = 3 → prints ***

i = 4 → prints ****

i = 5 → prints *****

✅ Sample Output
*
**
***
****
*****
