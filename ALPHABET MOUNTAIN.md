📘 README
Pattern Printing Program

Filename: Main.java
Language: Java

📋 Description

This program prints a character pyramid pattern using nested for loops.
It first prints characters A → D in an increasing triangle, then C → A in a decreasing triangle.

Pattern Output:

A
BB
CCC
DDDD
CCC
BB
A

⚙️ How It Works

The upper half has 4 rows:

Row 1 prints 1 A

Row 2 prints 2 B

Row 3 prints 3 C

Row 4 prints 4 D

The lower half has 3 rows:

Row 5 prints 3 C

Row 6 prints 2 B

Row 7 prints 1 A

Outer loop controls the number of rows.

Inner loop controls how many characters are printed in each row.

Character variable is incremented or decremented as needed.

▶️ How to Run

Save the code as Main.java.

Compile:

javac Main.java


Run:

java Main
```
public class Main {
    public static void main(String[] args) {
        // Upper half (increasing)
        char ch = 'A';
        for (int i = 1; i <= 4; i++) {
            for (int j = 1; j <= i; j++) {
                System.out.print(ch);
            }
            System.out.println();
            ch++;
        }

        // Lower half (decreasing)
        ch = 'C';
        for (int i = 3; i >= 1; i--) {
            for (int j = 1; j <= i; j++) {
                System.out.print(ch);
            }
            System.out.println();
            ch--;
        }
    }
}
```
