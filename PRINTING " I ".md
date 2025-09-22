Letter I Pattern in Java
📌 Description

This program prints the letter I using asterisks (*).
It uses nested for loops and conditional checks to form the horizontal and vertical bars of the letter I.

🖥️ Code Example
public class I {
    public static void main(String[] args) {
        int n = 10; // size of the letter

        for (int i = 0; i <= n; i++) {   // loop for rows
            for (int j = 0; j <= n; j++) {  // loop for columns

                // Conditions for "I"
                if (i == 0 || i == n || j == n/2) {
                    System.out.print("* ");
                } else {
                    System.out.print("  ");
                }
            }
            System.out.println(); // move to next line
        }
    }
}

🎯 Output (for n = 10)
* * * * * * * * * * 
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

Top Horizontal Bar → Printed when i == 0.

Bottom Horizontal Bar → Printed when i == n.

Vertical Line in the Middle → Printed when j == n/2.

Otherwise → Print spaces.
