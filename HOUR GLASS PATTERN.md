Diamond Pattern in Java

This program prints a diamond shape using stars (*).
The pattern is symmetric and formed by combining an inverted pyramid and an upright pyramid.

📌 Example Output (for n = 5)
 *********
  *******
   *****
    ***
     *
    ***
   *****
  *******
 *********

💻 Code
public class DiamondPattern {
    public static void main(String[] args) {
        int n = 5; // height of half diamond

        // Upper part (inverted pyramid)
        for (int i = 0; i < n; i++) {
            // spaces
            for (int j = 0; j < i; j++) {
                System.out.print(" ");
            }
            // stars
            for (int j = 0; j < 2 * (n - i) - 1; j++) {
                System.out.print("*");
            }
            System.out.println();
        }

        // Lower part (upright pyramid)
        for (int i = 1; i < n; i++) {
            // spaces
            for (int j = n - 1; j > i; j--) {
                System.out.print(" ");
            }
            // stars
            for (int j = 0; j < 2 * i + 1; j++) {
                System.out.print("*");
            }
            System.out.println();
        }
    }
}

🚀 How It Works

First loop → prints the top half (inverted pyramid).

Second loop → prints the bottom half (upright pyramid).

Together, they form a diamond pattern.

📝 Notes

You can change the value of n to make the diamond bigger or smaller.

For example:

n = 3 → smaller diamond

n = 7 → larger diamond
