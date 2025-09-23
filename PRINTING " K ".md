Letter K Pattern in Java
📌 Description

This program prints the letter K using asterisks (*).
It uses nested for loops and conditional checks to draw the vertical bar and diagonals of the letter K.

🖥️ Code Example
public class K {
    public static void main(String[] args) {
        int n = 10; // size of the letter

        for (int i = 0; i <= n; i++) {   // rows
            for (int j = 0; j <= n; j++) { // columns

                // Conditions for K
                if (j == 0 ||                // left vertical line
                    i + j == n/2 ||          // diagonal from top-left
                    i - j == n/2) {          // diagonal from bottom-left
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
*         *           
*       *             
*     *               
*   *                 
* *                   
*                     
* *                   
*   *                 
*     *               
*       *             
*         *          

⚙️ How It Works

Vertical Left Bar → Printed when j == 0.

Upper Diagonal → Printed when i + j == n/2.

Lower Diagonal → Printed when i - j == n/2.

Otherwise → Spaces are printed.

🚀 Usage

Compile:

javac K.java


Run:

java K


This will display the Letter K pattern on the console.
