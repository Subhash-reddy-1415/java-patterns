📌 Problem Statement

Write a Java program to print the following pattern:

1
12
123
1234
12345

📝 Explanation

The outer loop (i) runs from 1 to 5 → controls the number of rows.

The inner loop (j) runs from 1 to i → prints numbers in each row.

After finishing each row, System.out.println() moves the cursor to the next line.

💻 Code
```
public class Main {
    public static void main(String[] args) {
        // Outer loop for rows
        for (int i = 1; i <= 5; i++) {
            
            // Inner loop for printing numbers
            for (int j = 1; j <= i; j++) {
                System.out.print(j);
            }
            
            // Move to next line after each row
            System.out.println();
        }
    }
}
```

🔎 Dry Run

i = 1 → prints 1

i = 2 → prints 12

i = 3 → prints 123

i = 4 → prints 1234

i = 5 → prints 12345

✅ Sample Output
1
12
123
1234
12345
