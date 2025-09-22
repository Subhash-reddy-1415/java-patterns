Letter J Pattern in Java
📌 Description

This program prints the letter J using asterisks (*).
It uses nested for loops with conditional checks to form the top bar, vertical stem, bottom curve, and left hook of the letter J.

🖥️ Code Example
public class J {
    public static void main(String[] args) {
        int n = 10; // size of the letter

        for (int i = 0; i <= n; i++) {   // rows
            for (int j = 0; j <= n; j++) { // columns

                // Conditions for J
                if (i == 0 ||                // top horizontal line
                    j == n/2 ||              // vertical line in middle
                    (i == n && j <= n/2) ||  // bottom horizontal half
                    (j == 0 && i >= n/2)) {  // left hook
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
* * * * * * * * * * 
          * 
          * 
          * 
          * 
          * 
          * 
*         * 
*         * 
* * * * *   

⚙️ How It Works

Top Horizontal Bar → Printed when i == 0.

Vertical Middle Line → Printed when j == n/2.

Bottom Horizontal Hook → Printed when i == n && j <= n/2.

Left Hook → Printed when j == 0 && i >= n/2.

Otherwise → Print spaces.
