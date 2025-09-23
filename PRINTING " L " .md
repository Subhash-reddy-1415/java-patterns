Letter L Pattern in Java
📌 Description

This program prints the letter L using asterisks (*).
It uses nested loops to form the vertical and horizontal bars of the letter L.

🖥️ Code Example
public class L {
    public static void main(String[] args) {
        int n = 10; // size of the letter

        for (int i = 0; i <= n; i++) {   // rows
            for (int j = 0; j <= n; j++) { // columns

                // Conditions for L
                if (j == 0 || i == n) {   // left vertical line OR bottom horizontal line
                    System.out.print("* ");
                } else {
                    System.out.print("  ");
                }
            }
            System.out.println();
        }
    }
}

🎯 Output (for n = 10)
* 
* 
* 
* 
* 
* 
* 
* 
* 
* * * * * * * * * * 

⚙️ How It Works

Left Vertical Bar → Printed when j == 0.

Bottom Horizontal Bar → Printed when i == n.

Otherwise → Spaces are printed.

🚀 Usage

Compile:

javac L.java


Run:

java L


This will display the Letter L pattern on the console.
