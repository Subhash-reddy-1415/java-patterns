📌 Problem Statement

Write a Java program to print the following pattern using nested loops:

1111
2222
3333
4444

📝 Explanation

Use two loops:

Outer loop → controls the number of rows.

Inner loop → controls the number of columns.

For each row i, print the number i exactly 4 times.

After printing each row, move to the next line.

💻 Code
```
public class Main {
    public static void main(String[] args) {
        // Outer loop for rows
        for(int i = 1; i <= 4; i++) {
            
            // Inner loop for columns
            for(int j = 1; j <= 4; j++) {
                System.out.print(i); // Print row number
            }
            
            // Move to next line
            System.out.println();
        }
    }
}
```

🔎 Dry Run

i = 1 → prints 1111

i = 2 → prints 2222

i = 3 → prints 3333

i = 4 → prints 4444

✅ Sample Output
1111
2222
3333
4444
