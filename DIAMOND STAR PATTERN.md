Diamond Star Pattern in Java

This program prints a diamond shape using stars (*).
It uses two parts:

Upper Half → Pyramid of stars

Lower Half → Inverted pyramid of stars

📌 Example Output (for n = 5)
     *
    ***
   *****
  *******
 *********
  *******
   *****
    ***
     *

💻 Code
public class Pp {
    public static void main(String[] args) {
        // Upper half of diamond
        for (int i = 1; i <= 5; i++) {
            // spaces
            for (int j = 5; j >= i; j--) {
                System.out.print(" ");
            }
            // stars
            for (int j = 1; j <= 2 * i - 1; j++) {
                System.out.print("*");
            }
            System.out.println();
        }

        // Lower half of diamond
        for (int i = 2; i <= 5; i++) {
            // spaces
            for (int j = 1; j <= i; j++) {
                System.out.print(" ");
            }
            // stars
            for (int j = 1; j <= 11 - 2 * i; j++) {
                System.out.print("*");
            }
            System.out.println();
        }
    }
}

🚀 How It Works

First for loop → Prints the upper pyramid by decreasing spaces and increasing stars.

Second for loop → Prints the lower pyramid by increasing spaces and decreasing stars.

Together, they form a diamond.

📝 Notes

The diamond height depends on the loop limit (i <= 5).

You can modify the number 5 to generate bigger or smaller diamonds.
